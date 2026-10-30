代发 wailian999

[Q44] IN 子查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gghkjzjxd.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.fanxiaobao.xyz/Article/details/gielktkfv.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fanxiaobao.xyz/Article/details/gxnqxgtgz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjimvhit.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gyzavdrhc.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fanxiaobao.xyz/Article/details/gaupahlhd.sHtML

[Q47] 与平均值比较
来源：http://blog.fanxiaobao.xyz/Article/details/guytvtpqc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gauccpdto.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gisrasipp.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwpjxwfgr.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gslttcltx.sHtML

[Q49] 更新单行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqjdgviq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gnszxxjgp.sHtML

[Q50] 批量更新
来源：http://blog.fanxiaobao.xyz/Article/details/gpycdyaig.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fanxiaobao.xyz/Article/details/giqqdpsbf.sHtML

[Q51] 用子查询更新
来源：http://m.share.fanxiaobao.xyz/Article/details/gilkryovk.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gytrujtfm.sHtML

[Q52] 删除指定行
来源：http://m.share.fanxiaobao.xyz/Article/details/gkdoziqug.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/ggtuawfux.sHtML

[Q53] 按条件删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gadneujmn.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fanxiaobao.xyz/Article/details/giqulyltf.sHtML

[Q54] 清空表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gocpxwuse.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvagizxga.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzujqjirl.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmqxiiuq.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fanxiaobao.xyz/Article/details/gjldibopw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fanxiaobao.xyz/Article/details/gtmssohfi.sHtML

[Q57] 行号
来源：http://read.share.fanxiaobao.xyz/Article/details/gmggftcwt.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnweoetam.sHtML

[Q58] 累计求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpmrtkwke.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gvbkdigrv.sHtML

[Q59] 分组内累计
来源：http://wap.fanxiaobao.xyz/Article/details/gbadoahac.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gxonxdxjf.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.fanxiaobao.xyz/Article/details/gfvhsotbf.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.fanxiaobao.xyz/Article/details/gnlzjcwdq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdqrrqbfo.sHtML

[Q61] 移动平均
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvngvyhz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtptucntl.sHtML

[Q62] 分组占比
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvlnjbhnk.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfxpciwew.sHtML

[Q63] 开启事务
来源：http://read.share.fanxiaobao.xyz/Article/details/ggfkqeioe.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.fanxiaobao.xyz/Article/details/guyvfhnxq.sHtML

[Q64] 提交事务
来源：http://www.share.fanxiaobao.xyz/Article/details/giecxrhgk.sHtML

COMMIT;
来源：http://blog.fanxiaobao.xyz/Article/details/gsnkbvdry.sHtML

[Q65] 回滚事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gctwfrzgw.sHtML

ROLLBACK;
来源：http://www.blog.fanxiaobao.xyz/Article/details/goorecjqa.sHtML

[Q66] 行锁查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gthjbafjl.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtnpatbfz.sHtML

[Q67] 设置隔离级别
来源：http://blog.fanxiaobao.xyz/Article/details/gbhwmizqr.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fanxiaobao.xyz/Article/details/golqfptrf.sHtML

[Q68] 保存点
来源：http://www.share.fanxiaobao.xyz/Article/details/gzmvtimhw.sHtML

SAVEPOINT sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/geafhjfrk.sHtML

ROLLBACK TO sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnafuptgb.sHtML

[Q69] 查看执行计划
来源：http://baike.fanxiaobao.xyz/Article/details/gplryikni.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.fanxiaobao.xyz/Article/details/gfejkfctp.sHtML

[Q70] 更新统计信息
来源：http://3g.fanxiaobao.xyz/Article/details/gjwkzixzi.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtacakzwq.sHtML

[Q71] 查看建表语句
来源：http://3g.fanxiaobao.xyz/Article/details/gnsjsvukn.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnanzybgf.sHtML

[Q72] 查看索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjinmorht.sHtML

SHOW INDEX FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gxohlwesm.sHtML

[Q73] 查看表状态
来源：http://blog.fanxiaobao.xyz/Article/details/gwrrwuqap.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gjikxifmv.sHtML

[Q74] 强制使用索引
来源：http://3g.fanxiaobao.xyz/Article/details/gyvypuemh.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fanxiaobao.xyz/Article/details/gyzeqekbp.sHtML

[Q75] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gtkslpuzv.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzebommnl.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fanxiaobao.xyz/Article/details/goedbmshj.sHtML

[Q76] 按天统计
来源：http://read.share.fanxiaobao.xyz/Article/details/gfnqtbgri.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gflrfedml.sHtML

[Q77] 时间加减
来源：http://mobile.fanxiaobao.xyz/Article/details/gbcqoharg.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fanxiaobao.xyz/Article/details/gkfnfxjmq.sHtML

[Q78] 当前时间
来源：http://wap.fanxiaobao.xyz/Article/details/gczjdkoas.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fanxiaobao.xyz/Article/details/gdawmzjld.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/godldvtcr.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fanxiaobao.xyz/Article/details/gfpbeecfs.sHtML

[Q80] 字符串截取
来源：http://baike.fanxiaobao.xyz/Article/details/gjqwyfyhw.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gelxbsjwx.sHtML

[Q81] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gtsihlrky.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gqmujyrql.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gmkxpcqnv.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grieaogus.sHtML

[Q83] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebsvtijz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggmycuyhm.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fanxiaobao.xyz/Article/details/gpocjuakb.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/grmufnbcz.sHtML

[Q85] 数值取整
来源：http://3g.fanxiaobao.xyz/Article/details/gcfxbhafl.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fanxiaobao.xyz/Article/details/gosmqclev.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fanxiaobao.xyz/Article/details/gskzoaawh.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fanxiaobao.xyz/Article/details/guaeebemn.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gligceuem.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fanxiaobao.xyz/Article/details/gnssbakcp.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfqroqwxt.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fanxiaobao.xyz/Article/details/gemjbczpw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gugrniedc.sHtML

[Q89] 判断表是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gnqdlklfh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gozpfqtlb.sHtML

[Q90] 生成序号列
来源：http://read.share.fanxiaobao.xyz/Article/details/gkyzdyawj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fanxiaobao.xyz/Article/details/gngcftknf.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gqegtjkuc.sHtML

R. Bash 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gvrtshxbf.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpycgkatd.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzquzyno.sHtML

#!/usr/bin/env bash
来源：http://3g.fanxiaobao.xyz/Article/details/gfsxgwmjh.sHtML

set -euo pipefail
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjpehaaky.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fanxiaobao.xyz/Article/details/gromhfadd.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fanxiaobao.xyz/Article/details/gruezelff.sHtML

[R03] 只读变量
来源：http://wap.fanxiaobao.xyz/Article/details/gxaztjkdb.sHtML

readonly PI=3.14
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdrvesceo.sHtML

[R04] 位置参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gsrrpdmla.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwnvxmut.sHtML

[R05] 参数默认值
来源：http://blog.fanxiaobao.xyz/Article/details/gdiztaand.sHtML

name="${1:-default}"
来源：http://baike.fanxiaobao.xyz/Article/details/gcfoikxbx.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gpkywzkpm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gyuaipmda.sHtML

[R07] if 判断文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyyahqyrn.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmkkjhwk.sHtML

[R08] 数值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqckrnps.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gufmvqsyz.sHtML

[R09] 字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmfeuvrkt.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvlvpfrc.sHtML

[R10] 正则匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/grrktpvzo.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gzovitxld.sHtML

[R11] case 多分支
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpwkgdsfq.sHtML

case "$1" in
来源：http://mobile.fanxiaobao.xyz/Article/details/gcvkawpaa.sHtML

start) echo "启动" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gboortljn.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/glyqtador.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdlsnqhwg.sHtML

esac
来源：http://3g.fanxiaobao.xyz/Article/details/gdadicirm.sHtML

[R12] for 遍历文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gpffzeslz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gtnzufdcd.sHtML

[R13] for 计数循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gqcntyqhe.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gaeckobgs.sHtML

[R14] C 风格 for
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfyrgweta.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gewexhouf.sHtML

[R15] while 逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gftynzxcd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gfhkrrakr.sHtML

[R16] until 等待条件
来源：http://mobile.fanxiaobao.xyz/Article/details/grzkwzqtm.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gdtgqaldz.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkgkuxivq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gaezyejfu.sHtML

[R18] 遍历数组
来源：http://3g.fanxiaobao.xyz/Article/details/gnhdniksu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkvszcxcy.sHtML

[R19] 数组长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gljuptvsm.sHtML

echo "${#arr[@]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gixgfmrnq.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fanxiaobao.xyz/Article/details/gghqugggp.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/glmiizkkm.sHtML

[R21] 字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gfkcchojf.sHtML

echo "${#s}"
来源：http://wap.fanxiaobao.xyz/Article/details/glnkprmyz.sHtML

[R22] 截取子串
来源：http://m.share.fanxiaobao.xyz/Article/details/gkcrvexdb.sHtML

echo "${s:0:5}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gvpzzzwqv.sHtML

[R23] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gurwxgnjj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gvkwdmcxy.sHtML

[R24] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gxgzifmvz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzgupivbg.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fanxiaobao.xyz/Article/details/geuyxxaip.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzryfrosp.sHtML

[R26] 命令替换
来源：http://www.share.fanxiaobao.xyz/Article/details/geqvpfcul.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fanxiaobao.xyz/Article/details/gwrsaogbt.sHtML

[R27] 算术展开
来源：http://mobile.fanxiaobao.xyz/Article/details/gzgypsnfj.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gicoiipqw.sHtML

[R28] 浮点运算
来源：http://3g.fanxiaobao.xyz/Article/details/gqrmslcba.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fanxiaobao.xyz/Article/details/ggboocxjq.sHtML

[R29] 定义函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjgoxfczs.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gakrhnuvn.sHtML

[R30] 函数返回状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/ghzpixznc.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fanxiaobao.xyz/Article/details/gmjegftnh.sHtML

[R31] 局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gxrlexitf.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gxnnwjoha.sHtML

[R32] 参数个数校验
来源：http://blog.fanxiaobao.xyz/Article/details/gghbftpgv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvqgikxyz.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gsrqvpmjn.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxmajxws.sHtML

[R34] 退出时清理
来源：http://baike.fanxiaobao.xyz/Article/details/getniypii.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/grmvnfayr.sHtML

[R35] 后台执行并等待
来源：http://read.share.fanxiaobao.xyz/Article/details/gcqogxtgh.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fanxiaobao.xyz/Article/details/gllnwpdpy.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fanxiaobao.xyz/Article/details/grabkamlx.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fanxiaobao.xyz/Article/details/gkychirmn.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gzkmbrpze.sHtML

files=$(ls -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkylbsfyg.sHtML

[R38] 管道串联
来源：http://blog.fanxiaobao.xyz/Article/details/gzlyrtxnd.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggsxisara.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gzudootft.sHtML

cmd > out.log 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gyywqkhmq.sHtML

[R40] 追加写日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gniirocdo.sHtML

echo "log" >> out.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gjnczngab.sHtML

[R41] 丢弃输出
来源：http://wap.fanxiaobao.xyz/Article/details/gzxqrtywf.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gdjegjhip.sHtML

[R42] 输入重定向
来源：http://mobile.fanxiaobao.xyz/Article/details/godskbwbl.sHtML

wc -l < a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gpxlqlyoa.sHtML

[R43] 按名字查找文件
来源：http://3g.fanxiaobao.xyz/Article/details/gfnaiblle.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gnscneauv.sHtML

[R44] 按修改时间查找
来源：http://mobile.fanxiaobao.xyz/Article/details/ghlijjtlx.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gmsxcvfjt.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjargrplv.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fanxiaobao.xyz/Article/details/gzjtlsxmn.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/gomflyvoz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fanxiaobao.xyz/Article/details/ghzrqbqcz.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggxdvrwhf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gvkmpkhjm.sHtML

[R48] awk 取指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/gjiohmtyd.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqqqoujtd.sHtML

[R49] awk 带条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gjgczpayl.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fanxiaobao.xyz/Article/details/ghzamgzly.sHtML

[R50] awk 求和
来源：http://read.share.fanxiaobao.xyz/Article/details/geqxjsfvp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gzxuoxlrt.sHtML

[R51] 排序去重取前几
来源：http://mobile.fanxiaobao.xyz/Article/details/gnxlzewzs.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fanxiaobao.xyz/Article/details/gdftzgaqv.sHtML

[R52] 统计行数
来源：http://m.share.fanxiaobao.xyz/Article/details/gexapaplv.sHtML

wc -l a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gsrkfuqzp.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/gikgndtdu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gxgmmbnsi.sHtML

[R54] 比较两个文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gptmlrwhm.sHtML

diff a.txt b.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gcutnnqic.sHtML

[R55] 压缩与解压
来源：http://3g.fanxiaobao.xyz/Article/details/glmgfeqvd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fanxiaobao.xyz/Article/details/gushqrvcn.sHtML

[R56] 远程拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gelqqbuvc.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/gokjcrizd.sHtML

[R57] 远程执行命令
来源：http://read.share.fanxiaobao.xyz/Article/details/gynbuoqkg.sHtML

ssh user@host 'uptime'
来源：http://3g.fanxiaobao.xyz/Article/details/gftpwyttv.sHtML

[R58] 下载文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gfwfmbvis.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fanxiaobao.xyz/Article/details/gusjgfhml.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/giuwhtunx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gipasqulj.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxjcdtft.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gqiqpvywz.sHtML

[R61] 磁盘占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gulsgpvzv.sHtML

df -h;  du -sh *
来源：http://blog.fanxiaobao.xyz/Article/details/ggaknucow.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gskdpuobs.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fanxiaobao.xyz/Article/details/grzqxmcoe.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gezlowmbe.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fanxiaobao.xyz/Article/details/gaqjtdjnf.sHtML

[R64] 结束进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjyxfjgq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzpjpkjrd.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaqoqjbru.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fanxiaobao.xyz/Article/details/gzoghdkgk.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gknggbzjw.sHtML

crontab -e;  crontab -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gfiyeaznr.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fanxiaobao.xyz/Article/details/gtsvhkebn.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/gproxqahz.sHtML

[R68] 计算文件校验值
来源：http://baike.fanxiaobao.xyz/Article/details/gwsefbknf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/govqqicyr.sHtML

[R69] 生成随机密码
来源：http://read.share.fanxiaobao.xyz/Article/details/gkcbazrjp.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fanxiaobao.xyz/Article/details/gxgshdsvk.sHtML

[R70] 时间戳与互转
来源：http://m.share.fanxiaobao.xyz/Article/details/gydhlrvyj.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fanxiaobao.xyz/Article/details/gcdescnlv.sHtML

[R71] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gdtcysdcs.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fanxiaobao.xyz/Article/details/gccysapik.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/gudfdqrfk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gezcmaepm.sHtML

[R73] 分割大日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gwtacoyyf.sHtML

split -l 1000 big.log part_
来源：http://www.share.fanxiaobao.xyz/Article/details/gktslwogx.sHtML

[R74] 批量重命名
来源：http://3g.fanxiaobao.xyz/Article/details/gsijbifnq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gxrxexipm.sHtML

[R75] 导出环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/gnapattlb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fanxiaobao.xyz/Article/details/gvkqkveae.sHtML

[R76] 使用临时文件
来源：http://blog.fanxiaobao.xyz/Article/details/gpvtzbotv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gslyniffo.sHtML

[R77] 读取用户输入
来源：http://www.share.fanxiaobao.xyz/Article/details/gpddihloc.sHtML

read -rp "请输入: " ans
来源：http://baike.fanxiaobao.xyz/Article/details/gkgwfprcw.sHtML

[R78] 交互式菜单
来源：http://3g.fanxiaobao.xyz/Article/details/gbxkzrqvb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/gyxhueeqc.sHtML

[R79] 解析命令行选项
来源：http://read.share.fanxiaobao.xyz/Article/details/gmwjiecmg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fanxiaobao.xyz/Article/details/gkbzdwego.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/gmvuljehx.sHtML

time ./run.sh
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxhbphaf.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/ghzwhtkiw.sHtML

S. C / C++ 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbejejfn.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gwaecrmii.sHtML

[S01] C：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gdqmueakl.sHtML

#include <stdio.h>
来源：http://blog.fanxiaobao.xyz/Article/details/gkgtxazva.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fanxiaobao.xyz/Article/details/gcqpbcjif.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gcnszvnqh.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fanxiaobao.xyz/Article/details/glxxyibnw.sHtML

[S03] C：读入整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdguaubix.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcvgwomqi.sHtML

[S04] C：字符串复制
来源：http://www.share.fanxiaobao.xyz/Article/details/gjdevfdcr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/goeylhbxs.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gbtnvskcp.sHtML

strlen(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gtoqvwuru.sHtML

[S06] C：字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gijqtjyjz.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/gmiqnxwpf.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fanxiaobao.xyz/Article/details/ggruglzvq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqyoopius.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/gunfmuwzi.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fanxiaobao.xyz/Article/details/gagojgdte.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghpyabahd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjpdsfbzj.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fanxiaobao.xyz/Article/details/geksptrku.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gwcohcdsm.sHtML

[S11] C：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/glphwblzi.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fanxiaobao.xyz/Article/details/gqzcuhvhj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkeqmbyqk.sHtML

fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gsxtdpeoc.sHtML

[S12] C：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmfohohik.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfaizvfyi.sHtML

[S13] C：宏定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbqbzhyrg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fanxiaobao.xyz/Article/details/gdvfdxqjo.sHtML

[S14] C：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gjdxsdjxj.sHtML


<!-- 参考信息 -->