代发 wailian999

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3pgeeawvn.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3bwcsmhvi.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3gxqdnxyw.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3lbselilq.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ftnlunkx.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3lsfpnufz.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3hyswvgov.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3juekryqu.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3katyvbio.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3fmygftul.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3yiggusum.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3tlbqrkfq.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3fxllosmt.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3paimefdv.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3seywqxuz.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3wlyptntv.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3ljakbtpa.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3oiikuiri.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3tnvleniv.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3lfbbjbnj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gibmnsaf.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3efepxelw.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xaduhigx.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3kpsrzxjd.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jzcswhyq.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3ofojtqiv.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3ksyhalgz.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3sgbwyujj.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3wlgcqzds.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rkdtolph.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3dslhpfod.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ekqghpqp.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3eluyucfh.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3zcdcdohe.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3rttvgfmk.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3dyoddhdx.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3wwjeyncg.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3fektvjcd.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3jtipcats.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3oqudxlpd.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3rzglnwwo.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3sfnmyexm.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3kbuxdaxy.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3txajumqi.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3qgfyobbj.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3kyavyntq.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3lvzshwia.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3wodxxpwt.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3qbwgqmlv.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3dhmerhjs.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3rmbayhdi.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3tujekfxr.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3maplvtea.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3meargbdd.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3nikhcskg.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3kscapveg.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3ttopamam.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3loebpvmp.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jmpshbtr.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3vpznarue.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3bektfwsc.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3djrunexj.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3rmwxyben.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3vniyaqmr.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3shnhxodl.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3avhklreu.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3qqgnhhay.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3tptckpkj.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3lyvdbtoa.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ufbfkouv.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3hzwrqqca.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yppaqmvb.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3ynkfeyxm.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rsbuhbda.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3gwihrilu.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rgvzlsxc.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3xfejtxin.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hlttaoxg.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3kbcrggbe.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3crlxcnvc.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3hfqmgqtj.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3dfpzfjbk.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3mtefhfjx.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3arxcwrcn.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3szihbgdc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3zieovnps.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3knhyneuv.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3hyotadcg.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3etudtkei.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3qxqurzlv.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3iovqmxau.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3icdxicfs.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3jdwsfzxo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fngldkix.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3owgmzabv.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3nfrrgiir.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3oorimntt.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3tkywzxpt.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3ijmkjlqr.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3tfczkomr.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3tbrhmgqh.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3zwlqlhha.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3khqxqfxr.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3udqjiblm.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3wyjzqeup.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3zdskzzft.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3iocwzaqf.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3npuygtyi.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3hstzamzt.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3pbxysnvn.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3pnknkoea.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3cannredg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3bwsiemcf.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3iftcbzfl.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3tuvczofc.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3cyevkhdj.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3yiuzlgmh.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3eqmuiqcw.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3zngmvmmd.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3osceonlr.html

esac
来源：http://www.52xcode.cn/Article/details/gt3yvxvelvn.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3jezespjh.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3bqxjcjnx.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3cybubcti.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3myilyrlw.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3yieelhrn.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3zvienxkx.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3icbmxpfh.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3taafepqe.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3mqoutrxj.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3tspxqszm.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3rkpszhro.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3vzehtbbo.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3sabvmngg.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3fpfsdefu.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3ymjqikrr.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3dxxlzvuo.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3nmbjhids.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3rfjukmft.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3ltkkyhyh.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3pdvkifli.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3ipqdnufo.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3cgxzbczo.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3lywpgxcf.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3eqlnbjef.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3qophzgvp.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3xvgxirtq.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3gezlvbbt.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3qupqmxks.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3xeomprir.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3cgetpvjo.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3mpovahpw.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3rzxengun.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3rydwytnj.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3jqvlexhy.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3cxuybwby.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3rbidwbai.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3blacjaru.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3vprhjxwq.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3suvgzmwt.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3ylrxwqao.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3ezgpbjbg.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3iljzzivh.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3lbkmvgfu.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3pywwvwps.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3wuwjrafw.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3pxdcxwyh.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3gluapjpi.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3uhjwwhbu.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3zcxzgrlv.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3bqipaxcn.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3xhhtdcvo.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3wglkktpo.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3wsmewgdp.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3macnflbx.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3pypjhafq.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3aczmrycr.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3ojiiecly.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3uczlfvnk.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3ccspvzcq.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3xzqbkpza.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3doxvferz.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3btszqmys.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3dxnltgzo.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3hwgldpbm.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3uvblmwec.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3pdgthpgf.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3upkdykog.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3foycosop.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3qtjosseu.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3grhyxwnm.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3ksqbalrr.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3uszepejw.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3xfmwoajy.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3zpmthlhb.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3thydrsqk.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3rxhggvsi.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3gfeggyzy.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ajigamwj.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3jvcnysxe.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3jdmhlrwi.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3hcswsxpe.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wokgzzva.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3ujxyoxnj.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3vbbctiwl.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3uxroumyy.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3flwfpbgj.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3ysctnfke.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3igmplvxd.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ytmmarxh.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3dhppaclk.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3pbgibcjz.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3zslmodpr.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3vsscvaih.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3zmowwsxb.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3spfbneww.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3qtfxstry.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3ofgmzspt.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3pwxtkebf.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3mqchxtwf.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3slvjxpbi.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3iglmvxas.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3sbvczyif.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3nwbqoiju.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3cicxurrg.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3nduakmjl.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3abigbqnv.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3ttnpzfak.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3psybvpuq.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3mbybpegw.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3jzoxowpv.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3swexzkoy.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3ntymqzxy.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3uadllfor.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3inastonl.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3rcszdqub.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3sxhoocsf.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3mwbbkqep.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3juipvncq.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3vleqphyf.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3fidrktkn.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3ckmqocys.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3ccngycpx.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3zjxhzyeo.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3ozgsidbi.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3grheyqjh.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3zrrmockk.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3qetxpjye.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3kjkufdez.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3dykymnxo.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3kqufozne.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3txjzdemj.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3pgoqbmqg.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3fsoelkik.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3voghuhhj.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3mceceptl.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3tkgqaxzw.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3bojlxvvt.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3sfzcbihz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dgtmphji.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3woilwsum.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nefpfrmd.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ewhazzww.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3qgogxrmn.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3xzmlxzkf.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3xrljgxtl.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3tyinrmvs.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3iswkoief.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3nurcxndc.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3zscgpmac.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3rwooqean.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3cnnjvent.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3pssmadlq.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3fbldyiic.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3cswekrkw.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3ejlrcsrv.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3rayieslm.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3ionttysk.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3qdfhrfka.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3zykhcsqu.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3qdppzilm.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3keefnbgc.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3oaozwmvz.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ublpuvtd.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3ahkghrep.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3liujtzuq.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3oxutktfv.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3rztuhofk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3hfpusbka.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3nggryboj.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3insldnal.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3ggxclbgo.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3jvavngjw.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3rlpdtsmf.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3oszmskfr.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3rgcygtna.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3ebygvkjb.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kqvhfmfh.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3vnxsgkma.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3irlbpkbl.html


<!-- 参考信息 -->