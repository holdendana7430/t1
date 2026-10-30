代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://3g.fanxiaobao.xyz/Article/details/gyfefbiml.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzldlyitx.sHtML

[Q47] 与平均值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtftxdnbo.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fanxiaobao.xyz/Article/details/gqxzeoqly.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.fanxiaobao.xyz/Article/details/goifbgnkq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfdjsyalf.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gncvshiez.sHtML

[Q49] 更新单行
来源：http://read.share.fanxiaobao.xyz/Article/details/ghorwhyby.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gldvnrgpk.sHtML

[Q50] 批量更新
来源：http://wap.fanxiaobao.xyz/Article/details/glpnhrfwc.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fanxiaobao.xyz/Article/details/gjvlhywie.sHtML

[Q51] 用子查询更新
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjftbxvc.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gvdqmrdnv.sHtML

[Q52] 删除指定行
来源：http://baike.fanxiaobao.xyz/Article/details/gbbvkijgd.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbpnwdmyd.sHtML

[Q53] 按条件删除
来源：http://m.share.fanxiaobao.xyz/Article/details/gftnutjuk.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtjqjwfvb.sHtML

[Q54] 清空表
来源：http://read.share.fanxiaobao.xyz/Article/details/grgddnkrb.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fanxiaobao.xyz/Article/details/gbkzsyeue.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fanxiaobao.xyz/Article/details/gbvoettmq.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggpyfthue.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.fanxiaobao.xyz/Article/details/gmjblirun.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvtiopxki.sHtML

[Q57] 行号
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdylqzzo.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gwdewgfsp.sHtML

[Q58] 累计求和
来源：http://3g.fanxiaobao.xyz/Article/details/gyyofqhuw.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdggucsyo.sHtML

[Q59] 分组内累计
来源：http://wap.fanxiaobao.xyz/Article/details/gtkyaaajq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gmdhilxzq.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzxrivasb.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fanxiaobao.xyz/Article/details/gipbbdney.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/goyktgifb.sHtML

[Q61] 移动平均
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmvadtuxa.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gspasmpmr.sHtML

[Q62] 分组占比
来源：http://www.share.fanxiaobao.xyz/Article/details/gaymzkrms.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/gcrhateku.sHtML

[Q63] 开启事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gssftkcfl.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fanxiaobao.xyz/Article/details/grbpozbxv.sHtML

[Q64] 提交事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gifipbooq.sHtML

COMMIT;
来源：http://wap.fanxiaobao.xyz/Article/details/guotikrzp.sHtML

[Q65] 回滚事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqsmdpuad.sHtML

ROLLBACK;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpcpkdsmn.sHtML

[Q66] 行锁查询
来源：http://baike.fanxiaobao.xyz/Article/details/giisqtsan.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvauoppse.sHtML

[Q67] 设置隔离级别
来源：http://3g.fanxiaobao.xyz/Article/details/gngnxggvj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfnqjijas.sHtML

[Q68] 保存点
来源：http://baike.fanxiaobao.xyz/Article/details/gmcwuhtum.sHtML

SAVEPOINT sp1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gesvoobrl.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/giwixnywo.sHtML

[Q69] 查看执行计划
来源：http://baike.fanxiaobao.xyz/Article/details/gdwdkzznw.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fanxiaobao.xyz/Article/details/gxnghznck.sHtML

[Q70] 更新统计信息
来源：http://baike.fanxiaobao.xyz/Article/details/gazfacdpx.sHtML

ANALYZE TABLE users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gaqqtcevx.sHtML

[Q71] 查看建表语句
来源：http://wap.fanxiaobao.xyz/Article/details/gmxqgjreu.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwzwrtsc.sHtML

[Q72] 查看索引
来源：http://read.share.fanxiaobao.xyz/Article/details/ghibowbsy.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwepkgtto.sHtML

[Q73] 查看表状态
来源：http://m.share.fanxiaobao.xyz/Article/details/gneazyucp.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/galkervhd.sHtML

[Q74] 强制使用索引
来源：http://3g.fanxiaobao.xyz/Article/details/gfontnabr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fanxiaobao.xyz/Article/details/gosanjrje.sHtML

[Q75] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gyknfeame.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gbxqirchd.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fanxiaobao.xyz/Article/details/gmouilstc.sHtML

[Q76] 按天统计
来源：http://www.share.fanxiaobao.xyz/Article/details/gkracdzmd.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhvwcvtl.sHtML

[Q77] 时间加减
来源：http://mobile.fanxiaobao.xyz/Article/details/gwxxhaiqu.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gendddqmc.sHtML

[Q78] 当前时间
来源：http://baike.fanxiaobao.xyz/Article/details/gtewdpbdm.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fanxiaobao.xyz/Article/details/gvlkclzxp.sHtML

[Q79] 字符串拼接
来源：http://blog.fanxiaobao.xyz/Article/details/gdpiincrr.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fanxiaobao.xyz/Article/details/gldwndnkh.sHtML

[Q80] 字符串截取
来源：http://m.share.fanxiaobao.xyz/Article/details/gvkhvenhq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gktpixigx.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghequospd.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhpuwzfw.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkrhoawxu.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcmyvmzth.sHtML

[Q83] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gdbgngfnv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvvkmldrl.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvbehdqey.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbhbtmtcp.sHtML

[Q85] 数值取整
来源：http://blog.fanxiaobao.xyz/Article/details/gutyophgx.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fanxiaobao.xyz/Article/details/grhqudnur.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fanxiaobao.xyz/Article/details/gwnefigmg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fanxiaobao.xyz/Article/details/gpfovlobf.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gpbepnpyv.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyahqmicg.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fanxiaobao.xyz/Article/details/gbvsqgnmn.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fanxiaobao.xyz/Article/details/goxrkexmc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/geuvcgleh.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjqluyos.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gktagaamb.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozfmdjwu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fanxiaobao.xyz/Article/details/ggkqecyfq.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gjnidermx.sHtML

R. Bash 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gbmnlslyh.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gokqnivuc.sHtML

[R01] shebang 与严格模式
来源：http://baike.fanxiaobao.xyz/Article/details/gxkltsloa.sHtML

#!/usr/bin/env bash
来源：http://mobile.fanxiaobao.xyz/Article/details/geltlexca.sHtML

set -euo pipefail
来源：http://mobile.fanxiaobao.xyz/Article/details/gwiqaupft.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fanxiaobao.xyz/Article/details/gsaepjiub.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtzsnuncj.sHtML

[R03] 只读变量
来源：http://3g.fanxiaobao.xyz/Article/details/gjrneizrg.sHtML

readonly PI=3.14
来源：http://www.share.fanxiaobao.xyz/Article/details/gxoljdkhc.sHtML

[R04] 位置参数
来源：http://blog.fanxiaobao.xyz/Article/details/gupopfkxv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fanxiaobao.xyz/Article/details/gkrerhtbn.sHtML

[R05] 参数默认值
来源：http://read.share.fanxiaobao.xyz/Article/details/ghxtjmeen.sHtML

name="${1:-default}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gnmzykacs.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghlujroch.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfivexmqy.sHtML

[R07] if 判断文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gdrckynqv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/garkhnvrh.sHtML

[R08] 数值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/giqgisttw.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gukiiwjca.sHtML

[R09] 字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gbripwahk.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfsdxjxen.sHtML

[R10] 正则匹配
来源：http://blog.fanxiaobao.xyz/Article/details/giasqdkff.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guuthtrvm.sHtML

[R11] case 多分支
来源：http://baike.fanxiaobao.xyz/Article/details/gsdtnqqtd.sHtML

case "$1" in
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxmwinfn.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gddmvyovc.sHtML

stop)  echo "停止" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gwdeysixl.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/geiqfenwm.sHtML

esac
来源：http://wap.fanxiaobao.xyz/Article/details/grtofnzft.sHtML

[R12] for 遍历文件
来源：http://blog.fanxiaobao.xyz/Article/details/giefatwiu.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gthrnbspm.sHtML

[R13] for 计数循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gkzccnhdh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/ggluyjqls.sHtML

[R14] C 风格 for
来源：http://wap.fanxiaobao.xyz/Article/details/gfdfdbnfa.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gghjvedjt.sHtML

[R15] while 逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gojsluxit.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjwurhbj.sHtML

[R16] until 等待条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmbuarjy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gdawwtxre.sHtML

[R17] 数组定义与取值
来源：http://wap.fanxiaobao.xyz/Article/details/gxmmbukis.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtnuprbo.sHtML

[R18] 遍历数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjdlybrb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fanxiaobao.xyz/Article/details/ghwhqtpca.sHtML

[R19] 数组长度
来源：http://blog.fanxiaobao.xyz/Article/details/gccvagkra.sHtML

echo "${#arr[@]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gsglxogus.sHtML

[R20] 关联数组（字典）
来源：http://3g.fanxiaobao.xyz/Article/details/gceasupbk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gzsuitbvx.sHtML

[R21] 字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gckcgiiqn.sHtML

echo "${#s}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmleckki.sHtML

[R22] 截取子串
来源：http://3g.fanxiaobao.xyz/Article/details/gbxbjebhq.sHtML

echo "${s:0:5}"
来源：http://3g.fanxiaobao.xyz/Article/details/gmezjsgyi.sHtML

[R23] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gmsvsreha.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fanxiaobao.xyz/Article/details/gkckbcktm.sHtML

[R24] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gyqgqhwld.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gmxqyhglv.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fanxiaobao.xyz/Article/details/gjhawzfjh.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fanxiaobao.xyz/Article/details/glyfmgabp.sHtML

[R26] 命令替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfsbykdyd.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fanxiaobao.xyz/Article/details/gtxbdotcz.sHtML

[R27] 算术展开
来源：http://wap.fanxiaobao.xyz/Article/details/geryhnmzk.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fanxiaobao.xyz/Article/details/goskcdrnp.sHtML

[R28] 浮点运算
来源：http://3g.fanxiaobao.xyz/Article/details/gbvzcqfcn.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fanxiaobao.xyz/Article/details/gjuyuecyx.sHtML

[R29] 定义函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gubehofod.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gzywlwwxt.sHtML

[R30] 函数返回状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gnryijdln.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fanxiaobao.xyz/Article/details/gdvyouymb.sHtML

[R31] 局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gxnsteslb.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjprfybsi.sHtML

[R32] 参数个数校验
来源：http://www.share.fanxiaobao.xyz/Article/details/gyllwdmpz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gdcpqfiif.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhpmbbar.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fanxiaobao.xyz/Article/details/gymcnkxpm.sHtML

[R34] 退出时清理
来源：http://mobile.fanxiaobao.xyz/Article/details/gtnnujprg.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gprikvmsk.sHtML

[R35] 后台执行并等待
来源：http://wap.fanxiaobao.xyz/Article/details/gjqjrqgge.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fanxiaobao.xyz/Article/details/gwyrbvyvv.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdveedype.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fanxiaobao.xyz/Article/details/gnytujblx.sHtML

[R37] 把输出赋给变量
来源：http://baike.fanxiaobao.xyz/Article/details/gryhtquow.sHtML

files=$(ls -1)
来源：http://3g.fanxiaobao.xyz/Article/details/gqeitvfxu.sHtML

[R38] 管道串联
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsdhujphu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gwzevujcd.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gzegvyzix.sHtML

cmd > out.log 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gzujezbef.sHtML

[R40] 追加写日志
来源：http://baike.fanxiaobao.xyz/Article/details/gwxfnyjvh.sHtML

echo "log" >> out.log
来源：http://blog.fanxiaobao.xyz/Article/details/gtcrhbrst.sHtML

[R41] 丢弃输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnzbdjacg.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gcbhiddhe.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/gpabpzgxq.sHtML

wc -l < a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gotrrhrep.sHtML

[R43] 按名字查找文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gjlzvbixc.sHtML

find . -name "*.log" -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/goysfgwvm.sHtML

[R44] 按修改时间查找
来源：http://blog.fanxiaobao.xyz/Article/details/gthgzcuaq.sHtML

find . -mtime -7 -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gfocclfpc.sHtML

[R45] 批量删除
来源：http://blog.fanxiaobao.xyz/Article/details/gldqycpqs.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/gztmkyxuf.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbpqaihco.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fanxiaobao.xyz/Article/details/ggpxhhzjc.sHtML

[R47] sed 单行替换
来源：http://blog.fanxiaobao.xyz/Article/details/gphrwtzbb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/giptkcxag.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/grjjdwzmi.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqnjrqlp.sHtML

[R49] awk 带条件
来源：http://wap.fanxiaobao.xyz/Article/details/glbzghiye.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fanxiaobao.xyz/Article/details/gjrhqhxvz.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gszecwyco.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/golrwfjnc.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fanxiaobao.xyz/Article/details/giiwizost.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fanxiaobao.xyz/Article/details/gignmphqh.sHtML

[R52] 统计行数
来源：http://m.share.fanxiaobao.xyz/Article/details/gymzukhpf.sHtML

wc -l a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmcaqtqj.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fanxiaobao.xyz/Article/details/gciqjubiz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fanxiaobao.xyz/Article/details/gqtnuhhgz.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gbggufnzz.sHtML

diff a.txt b.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjdnvhzd.sHtML

[R55] 压缩与解压
来源：http://3g.fanxiaobao.xyz/Article/details/gqfhhopty.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fanxiaobao.xyz/Article/details/gkapniumk.sHtML

[R56] 远程拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/grrocokvl.sHtML

scp file user@host:/path/
来源：http://blog.fanxiaobao.xyz/Article/details/gjmjnxurr.sHtML

[R57] 远程执行命令
来源：http://baike.fanxiaobao.xyz/Article/details/gctllhrja.sHtML

ssh user@host 'uptime'
来源：http://blog.fanxiaobao.xyz/Article/details/gzjjnyeat.sHtML

[R58] 下载文件
来源：http://blog.fanxiaobao.xyz/Article/details/gtmqkwplz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/gzazdkllu.sHtML

[R59] 发 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gpsloqsrc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/giatpezdg.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fanxiaobao.xyz/Article/details/grlbqsibr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fanxiaobao.xyz/Article/details/glmetqpwy.sHtML

[R61] 磁盘占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gjyhzhhpv.sHtML

df -h;  du -sh *
来源：http://m.share.fanxiaobao.xyz/Article/details/glvddewqf.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gggrwrqkv.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fanxiaobao.xyz/Article/details/gwobycuyg.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gbsapxueh.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fanxiaobao.xyz/Article/details/guexmgesh.sHtML

[R64] 结束进程
来源：http://m.share.fanxiaobao.xyz/Article/details/ggnebwjih.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjkbtuygq.sHtML

[R65] 查看端口占用
来源：http://wap.fanxiaobao.xyz/Article/details/gsahamtzz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fanxiaobao.xyz/Article/details/gjzvirfbm.sHtML

[R66] 定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/grmogvouq.sHtML

crontab -e;  crontab -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gypkftqle.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fanxiaobao.xyz/Article/details/gfjddysua.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/gcnuogxuu.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkefmqzxp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhlbogon.sHtML

[R69] 生成随机密码
来源：http://mobile.fanxiaobao.xyz/Article/details/gaabxnryh.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxuriffs.sHtML

[R70] 时间戳与互转
来源：http://read.share.fanxiaobao.xyz/Article/details/goaokpsrd.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fanxiaobao.xyz/Article/details/gkgljjjbo.sHtML

[R71] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxvxscfuz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fanxiaobao.xyz/Article/details/gnoiidllj.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/gfycbeucd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gyeymwsin.sHtML

[R73] 分割大日志
来源：http://blog.fanxiaobao.xyz/Article/details/gcwfcodwa.sHtML

split -l 1000 big.log part_
来源：http://www.share.fanxiaobao.xyz/Article/details/gstcjklsm.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/ginrzfrii.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/genttlpcu.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gyxdlwicn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fanxiaobao.xyz/Article/details/ghfporipp.sHtML

[R76] 使用临时文件
来源：http://read.share.fanxiaobao.xyz/Article/details/geqsjeohz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gourehjsv.sHtML

[R77] 读取用户输入
来源：http://3g.fanxiaobao.xyz/Article/details/gpsnmnfap.sHtML

read -rp "请输入: " ans
来源：http://mobile.fanxiaobao.xyz/Article/details/gkiyuhakf.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/gwtvvufjf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gppxfwidx.sHtML

[R79] 解析命令行选项
来源：http://www.share.fanxiaobao.xyz/Article/details/gefnyelob.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fanxiaobao.xyz/Article/details/gohgelzlr.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fanxiaobao.xyz/Article/details/gmdhhoiva.sHtML

time ./run.sh
来源：http://wap.fanxiaobao.xyz/Article/details/grgzvvwqy.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gicinyckk.sHtML

S. C / C++ 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gmhcfuisy.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gpvabeshq.sHtML

[S01] C：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gjztavuzo.sHtML

#include <stdio.h>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjpqgrpwg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fanxiaobao.xyz/Article/details/gogvciuxx.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fanxiaobao.xyz/Article/details/golgsrzde.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grlzaheco.sHtML

[S03] C：读入整数
来源：http://baike.fanxiaobao.xyz/Article/details/ganjxpeku.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqctewjln.sHtML

[S04] C：字符串复制
来源：http://blog.fanxiaobao.xyz/Article/details/glrnihuwz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/gmskdgkhj.sHtML

[S05] C：字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gugsqmwmi.sHtML

strlen(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcqlqrgpp.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqyaehvr.sHtML

strcmp(a, b) == 0
来源：http://3g.fanxiaobao.xyz/Article/details/gbwaaoojl.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/gvnimvevt.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fanxiaobao.xyz/Article/details/gojxwdoej.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fanxiaobao.xyz/Article/details/gpomjmbrs.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fanxiaobao.xyz/Article/details/gepmnfyjo.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fanxiaobao.xyz/Article/details/gxvmfyvzz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fanxiaobao.xyz/Article/details/gwknctuqe.sHtML

[S10] C：指针与解引用
来源：http://read.share.fanxiaobao.xyz/Article/details/gxlwgardv.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwuwrsiah.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpxvjsdaz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gicxehtis.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gapzztxio.sHtML

fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gftkezdsg.sHtML

[S12] C：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gcrfkxokd.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbouvxnva.sHtML

[S13] C：宏定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gzslcmkrc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fanxiaobao.xyz/Article/details/glnrkrqty.sHtML

[S14] C：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gatxttrfy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjucczzh.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gwesiwdsp.sHtML

(double) a / b
来源：http://3g.fanxiaobao.xyz/Article/details/gzsweioid.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/gyrnorufp.sHtML


<!-- 参考信息 -->