代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3irliarlv.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3tganysvr.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3qglzufrz.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3qmylnxyl.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3cxyqlhuv.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3qydnubkb.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3ypydzjsj.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3kpkueiaf.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3lugvugpw.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3aqgkejiu.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3shshvyvk.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3cazqigeo.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3tomzrmvf.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3twseuxgi.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3vpazlggd.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3uhuhouus.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3llsgbuqt.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3gbfavjxz.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3kzloncob.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3znlysyck.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3gzjslbgf.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3taalvpmv.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3jcoxdecu.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3fvrpdlne.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cfdeyfbd.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3lwynetjx.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qlwbbayw.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3zhyiddwh.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3agdpdley.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3dygxcddz.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3anofccty.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ilyhfvya.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3jkwzywwa.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3roontwpj.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3fedyezim.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3otyiipei.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3tqmozxdh.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3ndheiedz.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3dzuozebd.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3fgqojvxm.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3upeqtlvu.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3gxuogbdd.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3ostpkwfc.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3ktwodpxs.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3joivkbaa.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3inkfpbyl.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3dtzdikay.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3nojqyfch.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3cunvmrin.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3txkuizur.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3culxrbaj.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3doqxpspc.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3boppkkcw.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3jdnytjss.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3rubcwear.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3wezlewcx.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rjodxtsn.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3ftdlcnje.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3gycsveca.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3iugcctmq.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3vmmluoov.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3odgiugrg.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3dubnugqs.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3gqzpjldi.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3fgodyzkx.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3eximjwqf.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3jegmquyk.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3pplptmpp.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3zenahujr.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3ovvzilff.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3gpguwkkr.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3jmxyappr.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3yossqwso.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lyzylmmd.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3yqcvddkf.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3iphddgam.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3fothwcdt.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bwozzepc.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ecdyswek.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pxqslbxo.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3actqaecl.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bzmhtqbp.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3suizrolx.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3xpgowwzw.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3oqfzijjt.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3npnzbwbx.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3suoinsmd.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3zhmiwoal.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3vjvaxdue.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3svswcxea.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kjbsdtbz.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3plajvfii.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3mjxwrhtj.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3zfyyhwin.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3flblszgi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nhjjczok.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3bcgmxzcw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vzlcnkro.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3fyvrcfbg.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3lotoebhj.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3ogldfmlc.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3hzsocgqs.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3nluhgpnx.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3xkloypxg.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3mcsruduf.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3aqnozkli.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3ezuqjevb.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ecyihlvs.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3mjeeqzic.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3qivmaovl.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3chlnbnwh.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3mqvlakeg.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3wkvgddko.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3brvcyomh.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3xspjraur.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3zjxmmzsx.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3mtafnbnc.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3aqpnthxo.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3jdkpmtwm.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3lbnokkiw.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3bnhkxzgo.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3hqgczfze.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3eqatnkmz.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3nzsaytfv.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3xvbxymtq.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3cujcrsay.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3sqjnjbuh.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3nmvztyru.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3edxsdxwm.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3lgfmacof.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3nuokoytm.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3tzcfvfhx.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ggcrienz.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3eovqryao.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3dabrsfpe.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3yucncfey.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3ccwgdvjt.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3cqbywexd.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3iinpmfqn.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3xqszkgxn.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3exesswij.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3iidopuvv.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3rbioavwg.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3tylikrat.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3jarvpzyo.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3cgxuyvgs.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3vrcxpcof.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3dlvhmfqa.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3qbrhhbzd.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3qcfxjwoz.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3joecuzda.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3bdpbdknu.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3qnpcjiyc.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3vadjfnkt.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3wkzlqwwa.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3nhcigeda.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3iowgklwo.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3aaufxksd.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3ivtuoiqt.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3tsxxbxpe.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3zbimhdhl.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3ddfslryf.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3kexokyod.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3sfrgqxqo.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gtouiimg.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3dqebdnxd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3hwxnxlmy.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3fzxmlbzu.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3chcbotyy.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3nsjhkofj.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3btvbrdtu.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3oozjutch.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3xgosuffq.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3bhqmqlrh.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3ghxykrex.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3veebkqln.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3ouzpladc.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3bemfwddg.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3gyxflhvm.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3yfwkioii.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3ifulrsuf.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3rmtgeuos.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3uxdoelfq.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3jdrgkutt.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3qvhiyncl.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3dzfupgce.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3sbtkkqhc.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3amtecevp.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3cuxkgnic.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3kvjdihyv.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3zgipovdz.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3tlwmfmqk.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3tnctbayy.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3veesrugn.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3luoespwm.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3phnycezp.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3cfetzkaf.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3ezsgjzuz.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3svjcngxz.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3ajogevfb.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3hyifggdw.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3qsadkklu.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ermzxdms.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3asilixac.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3saqqlhdb.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3gecwetxm.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3mgniysnp.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3zmzjhcpr.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3tjmiufgy.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3okfrxcrn.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3ftwccfzr.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3wsdcaemr.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3urxqdedd.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3yhyskzry.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3rjmnqcia.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3hxoiexar.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3mmferdfr.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3weafdedy.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3isnhovud.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3zhcbjfpq.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3npmhokqo.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3jfefdjhm.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3uplcrkuz.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3dcktukxk.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3zudtydtc.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3fuhtvkao.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3bphwjlrz.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3hvmsrbum.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3oqghqvay.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3brpvfhdg.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3lxuikrej.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3watsxpva.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3lzzzceed.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3zhkjpsal.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3ulcwnbgo.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3fmdutond.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3cnloprqb.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3otwdguht.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3xxegwzkd.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3pancytwv.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3omkbvxkq.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3sixtiuyd.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3auxdttbn.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ymapaqua.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3rwwaizxu.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3vvhgukai.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3sxdtuynt.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3tkthbxgh.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3cvawmqrr.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3hnislhuk.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3nqlpyxrs.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ftdgvazi.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3bscdqqig.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3sbhgrktq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3revoykxj.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3gjsxfeow.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3hcqrlgoq.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3joktqztz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3icuoexov.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3dspvqidt.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3qicpnlmq.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3apduuywu.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3bblrkvxi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lribaxnr.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3mzwgcfyg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bpnmysmt.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ycnymuaf.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3stapxall.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3yfhwtbbo.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3pqwfqahn.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3klzdllpu.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3ntkmzemj.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3kmrdscam.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3rffwsbiw.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3doaoxfpk.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3aucrfgco.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3glfvkwjv.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3gvwuqewd.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3uclrioun.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3iibkvpzd.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3qvekbfxb.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3rdpuoxkb.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3thxxeuzj.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3ajbgbwqb.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3iugfnycx.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3ooexggkv.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3oqdzznpp.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3mizglfte.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3tuzpyitq.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3frlzgwfn.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3shfuqcfl.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3yrncfscd.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3abhiffsl.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3uuclrtrb.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3cxcmapdp.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3krwswiyy.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3awinrpqh.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3ypmvsegp.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3bycwdpub.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3vpkedjid.html


<!-- 参考信息 -->