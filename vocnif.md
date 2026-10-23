代发 wailian999

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ibluelvo.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3yquzgrop.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3yjbbytif.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3qfrcokol.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3bmnejnxp.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3asnyczuu.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3dpdxjwwq.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3avkdujmy.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3nsrlxafq.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3sftfpgxe.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3pbxqamwn.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3dbaazfzs.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3aphnhbbs.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3szvkyhed.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3eetlxfdu.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3hbzhodro.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3kxfgqhiz.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3tkplimdz.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3ovxigwmi.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3izgdxunt.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3naurbmco.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3qllngben.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3heetqlkw.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3dcdrgico.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3rxyvtqar.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3ddiyyvvd.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3frcpztvh.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3kxmmmgui.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3yxhvlgmi.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3whngqrbs.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3dsabuhlk.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3jhtkzlxr.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3lnwyzvfe.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3bmsyvooe.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3kjnjvkec.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3lcesyhme.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3zdgfgcwj.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3hsdtqinv.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3ghvpdrlp.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3iwdsifrm.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3rwkfhkfp.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3ietajtaq.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3kgwfnrcu.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3ehtbkfax.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3frdttiux.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3gneighsj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3prmvokdz.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3spbyfnhx.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3pfzhxfaa.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3ydosduzy.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3cvygcokv.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3agugnnhg.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tzldhqhn.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3mnfgaccf.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3trtlvvfi.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3xfcefono.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3ofnobxrl.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3bwyadktg.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xuilohgu.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3zqkthksc.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3duadkgwd.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3yfkubkit.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3yvwiinmg.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3qxpdmdhq.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3twkktogm.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3lsjiljeq.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3snyrlacp.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3euttwbyc.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3vdgxktvl.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dnwlbzvb.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3rjbstgrz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tsecrsjt.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3metnmief.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zqwgmdvy.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3kmatpybt.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wwqlzmkr.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3tjhjutsx.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3feeemazh.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3uoimwwwj.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3fdyomyqn.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3fezljvap.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3suzyceis.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3uiyvmqkr.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3ftgrixeg.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3cqqxozmj.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3uiajmlue.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vbtzjwim.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3pfuwasas.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3xtfcrwiy.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3uajyiyvw.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3fczfwqgv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gkworxcr.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3xqcubvzx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3diybiqzs.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3ldhiqqlq.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3iybeaeoe.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3krqmwiyp.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3trmlhrys.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3mbqjzjmh.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3ozhirnas.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3zvuujybf.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3txjwasyy.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3arcqaqyd.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3xfwytotb.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3vxyhgzvk.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3cydjelin.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3nfglqald.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3vstgagxp.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3gadsuybr.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3vjwqkuqm.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3qwreonkb.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3bvfmoutk.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3pqimbueu.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3czrkpyuo.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3wevbynug.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3qaflhfgu.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3yholqcsl.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3gtjckujf.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3fmorluus.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3hmzafgvk.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3gfqoxlmo.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3lhctdgco.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3oowspfdu.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3efnoodae.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3mdqphxhg.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3jjjqwnem.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3eqtgiejl.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3owkkosxa.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3rvpgodgb.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3megburvi.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3cqjnqeiy.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3mgjwddck.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3tdekqkxj.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3exyytjzl.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3cinvdufp.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3cjzbgtwl.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3clrhrrdq.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3mypmvgtm.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3sbdtwbld.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3bjjspnqt.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3viwctoaw.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3mwqoyixy.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3cijpmwnq.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3gclvqzyh.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3fiesqtbf.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ndsjoplc.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3yfayjawp.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3fnyjjmwq.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3zyiutpqm.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3gklelajq.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3etfjgfox.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3wpamxpok.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3laffpttj.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3qltcjmqa.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3bmwhkiec.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3nwestods.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3ksbmjjsr.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3jxxdiujw.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3lurplrtz.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3nhqmcdng.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3jratxhjf.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3kqliozug.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3ocdmxvtk.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3pjitnkxs.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3cvpvdyxp.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3sdfixwgd.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3zuimcqrl.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3ihaubydu.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3hffxjukv.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3qqaaimsn.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3pnsmxkzh.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3iinijyhh.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3dowmxukd.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3wavtfmdy.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3qkothvhd.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3vweiwiwz.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3krnrvgul.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3fxyygexl.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3jvxhloao.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3fpszlhkh.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3jbtpakdh.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3wwtmroqw.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3amvsvdbk.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3jopjslbw.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3ftsiqjzl.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3whhqwtkc.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3mznfzoei.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3yuhmewel.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3intkvvqk.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3kewfwidd.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3zpascenc.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3uypsgosz.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kknqpknb.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3lafcyqei.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ennzrmow.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3noaerhnh.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3jodfanrg.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3amiikpsh.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ivttkuvv.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3kzqppmmu.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3rzchvcjj.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3kfnxnmtx.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nnzgorhe.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3ilnsboht.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3qbxemqcp.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3hxcohhhh.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3exshmsrk.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3qplxqmpt.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3whziwiwr.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3leadnuvu.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3nerpleic.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3tajyaijp.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3xkbcgkbp.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3bxruftke.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3lhfpqcuv.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3ynkyowfp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3stwvqfql.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3npyblzyd.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3lszdlbku.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3hhsldecj.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3qgrdlkhf.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3bkfekynr.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3wansdctn.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3sxibwjwx.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3yujxnzkt.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3dkkyjuxw.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3cycqbdvi.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3pytefxfo.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3hyjmwbhm.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3vzsddftq.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3dktkunzo.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3ytjxkhod.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3mqthrmxw.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3ztigkkng.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kkgqofoc.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3ojugjfad.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3tzlbtszk.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3iecvhvdd.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3idkxwqdk.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3lpkfbhbb.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3uijedruq.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3hzikwhxa.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3ngyiksyz.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3ktroexrf.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3mmajlqtc.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3dijbvhps.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3zltdpwvk.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3qfcnzdno.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3ervpndou.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3rmzvmngv.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3nujgefxc.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3klsbqvco.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3jgquuwhf.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3npthjztr.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3tdfcnfct.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3eznsdudf.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3sppqehgg.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3ehovnlof.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3gabatmpf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uapjpsbp.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3rrmbgnqk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uzclfikp.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qcprrlwf.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3pjmkupet.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3yrsbimgg.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3rclrzhbx.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3vapbzuop.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3wzalzjou.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3zjxmtudu.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3zbjqduiw.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3iafuqlwy.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3irshazrs.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3cqcovcju.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3digoimhk.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3jnatebla.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3pfzwrhyz.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3poahcxgr.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3slbapcor.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3mnnohwgs.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3grguwach.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3szvtnfot.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3ydgtiqzw.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3gnimoqos.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3xfkyadmy.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3vrcsjmob.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3djpbcdzf.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3trmetuvw.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3orzcihrr.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3vburbbcv.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3vjlozpkr.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3gatqticv.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3ulzpkefb.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3uiibgbca.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3uycyltbp.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3bfdvxzbr.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3ejvxtxqb.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3oltwugqu.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3qwekicyw.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3lsefepbo.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3rtgzqnhm.html


<!-- 参考信息 -->