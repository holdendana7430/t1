代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3ntmrqdnp.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3dfczmkqt.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3lbnvtuis.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3bdirjmyv.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3riiwhsvk.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3frlwykeg.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3jhlkmiit.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3ghaqjzew.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3jseciecy.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3fkisgvdz.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3dnxjhabf.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3qsgjdokb.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3imkozllo.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3jkcndfvh.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3qykemgxx.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3htonbmsd.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3zovnlcxs.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3kpqkhatr.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3aatjekdn.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3vyymsyaj.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3aptllcpy.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3dfjrtkke.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3vkqkmvlt.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3gnctxska.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xwiyaynx.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3goexdotz.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3keilabcx.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3pkuzjocl.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qcwecwct.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3slzsgzfv.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3xwwgfjgf.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3bykblhnx.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3suhlwoag.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3qdnxwgpa.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3pwfpjrvb.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3kxlpipfr.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3tjahdnsi.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3phbtsgrg.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3bzzshknl.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3sjrmwtfu.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3yzoqcyyj.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3yylpkfhe.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3qfxnysaw.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3mkkvizbc.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3zndpxnkc.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3zzmzfdks.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3cfmbxrlk.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3tzauiios.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3evubqtyj.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3tfiepntn.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3iwdnscwh.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3ehavnkcf.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3yczahlbi.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3gbhxriud.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3mjqknume.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3lsnhbtnf.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vokxtmyn.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3fllahtik.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3mxwhciju.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3xnctlzrr.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3eckrvlfk.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3hnjnlakf.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3cpxbxyuv.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3wqszscfx.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3rixqorcf.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3agredngn.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3iydqdnzr.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3yuqtkzpq.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3aakzunld.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3hkfenoqo.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3lpoaujbu.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3gqzyzjhi.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3gfavxpok.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lpxuviag.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3sbfdaafq.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3podctftw.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3usnctken.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jmjpvdwj.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3eqgwwvfn.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uykzmmxg.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3wrkkzuas.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uqxjrofq.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3hfhdmilh.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3aohlolbx.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3ygjnobat.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3dwlolsyy.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3rczlhscn.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3vufutvnc.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3lyhutyhf.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3zccszkje.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3obdeesmd.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3wrscepmh.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3vzmuqbtx.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3nookijoa.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3rlndjxmx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xasnkfaf.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3phcdvemd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tcfefasv.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3lljiptxu.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3wahgkqrx.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3izptnbix.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3lxtqgcuy.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3pvzlfmdn.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3nhpfmkgs.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3tivewekc.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3ygrekbaa.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3kvnoaofy.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3gwpwwpbt.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3nyziucav.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3tgjumgjn.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3vbceurpu.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3vdaqzdyo.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3xukdkssa.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3hdykpzwh.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3trclyoce.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3tpmydrli.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3cychuxvp.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3hzezqgsy.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3lqtmwaph.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3jixctmid.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3txgkntfk.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3ouidqfav.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3ydoxycvv.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3xqqrtagd.html

esac
来源：http://www.52xcode.cn/Article/details/gt3wonlxrin.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3pcamdeyv.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3dkdyqawb.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3ufztpjoc.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3bslpoury.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3rugsvmdr.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3hkiyzaum.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3hllusxol.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hekygjos.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3rwjydowj.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3dyhnfash.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3vztnukkl.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3xrntznbk.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3hnykstlh.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3nybjedbz.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3uqkaxryq.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3crsmemct.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3zyztkhgs.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3lwofrghg.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3pnpzcfkv.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3dhvvuhal.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3gxxywvij.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3btiucvit.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3dnuheoqe.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3cwyjufck.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3eafwlsru.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3amvgyjey.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3teaqnwgm.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3hduirsum.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3bzarxjao.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3wgbceilj.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3vfjavmwy.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3vimknrda.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3aaagfrml.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3qotvaktm.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3bugjwfne.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3pgfrtfsy.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3zsqfvnvt.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3xsngghqw.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3gwikgimg.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3qggtuwuy.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3tctoblss.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3dhzxhfab.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3zprkdgws.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3sxflmgug.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3noobzfrq.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3edxpsdku.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3xcgrtfer.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3baobuubq.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3migcsaxm.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3jnmeiikf.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3gofvoliz.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3enxxxffq.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3qooijwtz.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3dainnrsw.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3cjbffgjy.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3olpsjddh.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3zgtoumnc.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3yrubiegr.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3tqextbli.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3tvedwbyi.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3wlwwboaw.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3almsxkmz.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3tajnfppj.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3yugeimtj.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3qiqcddnw.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3oophtami.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3jiffwzel.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3tioiylby.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3npzkgpep.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3wujrhrzu.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3upzluzal.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qpdkftuo.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3shqnqhjf.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gdfgdqoi.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3cobarlyn.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3vigfsmwh.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3eahpgdil.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3jtwywrqi.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3cesoleqa.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3afvylegd.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3cddldiex.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3pnjkfuzu.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3okdxknjo.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3hrzifsli.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3herdidly.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3twckmxlc.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3xjpshtit.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3qiaytnlh.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ksmgdgsq.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3jplzqujj.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3rseoekte.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3cnqpvumn.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3jmsoozon.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3hihcckia.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3ljlnocwq.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3oukarwli.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3mozgwtwq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3nearzbgq.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3wqrcvvto.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3bbcbjonm.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3wkwlpnjb.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3eglbnhiv.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3iztqrxci.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3alzzlsdc.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3afmuvszg.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3uzcgqutw.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3fjtruuls.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3bpdenfoz.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3xwxtvjdq.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3hmchyrkr.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3bkdjbjhu.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3lrvtegsh.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3bfsycqnn.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3omkztyas.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3gcxfcxjb.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3brofpoqd.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3ortuibzd.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3zzkueekp.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3vhoeomab.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3tzyomrcy.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3zqblncij.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3rugfecsk.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3cotqwtck.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3skvyyoxj.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3bcaqyfhr.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3dxlxuggy.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3mkoxctzi.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3xbjoqvxp.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3sdcbjobu.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3wglirfph.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3muhcsdru.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3iukbsthv.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3xafiqdll.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3kuhyihof.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3meotxfob.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3lduqskts.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3tsdyfsbf.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3fcrbeyiq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wnxykfaq.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3nidsyxwj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zoaqwkui.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ajyywxzn.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3sbhzaked.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3tlalalhg.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3ymfmagxc.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3wynzbliv.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3ovtqqbkf.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3guyktils.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3jjbgzyqt.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3zbbmdwqq.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3inhfcbve.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qkgvomme.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3zwfvxskq.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3tzonelur.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3jecloehg.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3kquoxgka.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3klursbhe.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3mzfpnysh.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3xnpvngsa.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3ntotimic.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3gictfqmd.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3rsdsiouz.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3dpfrffmw.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3zlowkhbh.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3vbrlbkoz.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3telzrmjn.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3fgrmyprc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3lzjfkdab.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3xqsbmbip.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3igqiobpf.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3mjqcmtbq.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3ayxilsdk.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3vtpkkiaq.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3yctomdeq.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3vgnfnsdp.html


<!-- 参考信息 -->