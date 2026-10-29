代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.hesvh.cn/Article/details/gbowricjb.sHtML

[Q52] 删除指定行
来源：http://m.share.zdbjq.cn/Article/details/ghtvypkqw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gdkmvouhx.sHtML

[Q53] 按条件删除
来源：http://www.share.fehbvm.com/Article/details/gtawdtpqh.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.hesvh.cn/Article/details/goljnlsqt.sHtML

[Q54] 清空表
来源：http://baike.hesvh.cn/Article/details/gqgiwyjqb.sHtML

TRUNCATE TABLE logs;
来源：http://wap.hesvh.cn/Article/details/gmzsfoiki.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fehbvm.com/Article/details/gitwyukuz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.hesvh.cn/Article/details/gvhovzcou.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.hesvh.cn/Article/details/gjfkqgjjq.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fehbvm.com/Article/details/gkmtzcmio.sHtML

[Q57] 行号
来源：http://www.share.fehbvm.com/Article/details/gctmpuzbi.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fehbvm.com/Article/details/grnlwjjcq.sHtML

[Q58] 累计求和
来源：http://baike.hesvh.cn/Article/details/glggyrizn.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/ghwwygwjm.sHtML

[Q59] 分组内累计
来源：http://3g.zdbjq.cn/Article/details/gdfovlgyp.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.hesvh.cn/Article/details/geyjrgoiq.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fehbvm.com/Article/details/gdwsnewci.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fehbvm.com/Article/details/gfekzpbgb.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gwxoiirbx.sHtML

[Q61] 移动平均
来源：http://wap.zdbjq.cn/Article/details/gwnacyanj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/ghqfclwbq.sHtML

[Q62] 分组占比
来源：http://www.share.zdbjq.cn/Article/details/gjcmvagoh.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/guhyrmtst.sHtML

[Q63] 开启事务
来源：http://baike.hesvh.cn/Article/details/gkqzghjfh.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.zdbjq.cn/Article/details/glxdhhigz.sHtML

[Q64] 提交事务
来源：http://blog.fehbvm.com/Article/details/gdufefgic.sHtML

COMMIT;
来源：http://www.m.share.fehbvm.com/Article/details/ggpdmmlyr.sHtML

[Q65] 回滚事务
来源：http://m.share.fehbvm.com/Article/details/gscmhcbxm.sHtML

ROLLBACK;
来源：http://read.share.zdbjq.cn/Article/details/giykujnsq.sHtML

[Q66] 行锁查询
来源：http://www.blog.zdbjq.cn/Article/details/gkryuphuj.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.zdbjq.cn/Article/details/gycuchtka.sHtML

[Q67] 设置隔离级别
来源：http://blog.zdbjq.cn/Article/details/gpameljow.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.zdbjq.cn/Article/details/ghmugdmts.sHtML

[Q68] 保存点
来源：http://wap.zdbjq.cn/Article/details/gfrgyuyoj.sHtML

SAVEPOINT sp1;
来源：http://wap.zdbjq.cn/Article/details/gvfzigpfe.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.hesvh.cn/Article/details/geutoexqk.sHtML

[Q69] 查看执行计划
来源：http://baike.fehbvm.com/Article/details/gqzrevywo.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.zdbjq.cn/Article/details/gdbxfnsid.sHtML

[Q70] 更新统计信息
来源：http://m.share.zdbjq.cn/Article/details/gaoxkgccz.sHtML

ANALYZE TABLE users;
来源：http://mobile.zdbjq.cn/Article/details/gczpgqrln.sHtML

[Q71] 查看建表语句
来源：http://3g.fehbvm.com/Article/details/ggbxurpiz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.hesvh.cn/Article/details/gbbmfnboj.sHtML

[Q72] 查看索引
来源：http://read.share.zdbjq.cn/Article/details/godymdlpc.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gbodktknb.sHtML

[Q73] 查看表状态
来源：http://blog.hesvh.cn/Article/details/gppolagrv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/grrprkobj.sHtML

[Q74] 强制使用索引
来源：http://blog.hesvh.cn/Article/details/gfulzhxkv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fehbvm.com/Article/details/gezpmmhlx.sHtML

[Q75] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gvmbjqfsz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.zdbjq.cn/Article/details/grwvaidhz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fehbvm.com/Article/details/gteolapcf.sHtML

[Q76] 按天统计
来源：http://3g.hesvh.cn/Article/details/givgvtxre.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.zdbjq.cn/Article/details/gwvcjffgj.sHtML

[Q77] 时间加减
来源：http://3g.zdbjq.cn/Article/details/gjpdnlkhk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.zdbjq.cn/Article/details/gscmjxlug.sHtML

[Q78] 当前时间
来源：http://3g.zdbjq.cn/Article/details/gzsfndmfp.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fehbvm.com/Article/details/gmgyejntz.sHtML

[Q79] 字符串拼接
来源：http://www.share.fehbvm.com/Article/details/grxmlhjqt.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fehbvm.com/Article/details/gxvxoxsig.sHtML

[Q80] 字符串截取
来源：http://read.share.hesvh.cn/Article/details/gmbgjlpfg.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fehbvm.com/Article/details/grchygian.sHtML

[Q81] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/gpeaziina.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fehbvm.com/Article/details/gxevkcmvq.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.zdbjq.cn/Article/details/gxpmvotck.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gxjalmfgu.sHtML

[Q83] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gwardkvtc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gxrqzgqfu.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fehbvm.com/Article/details/gkymzfmha.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gdxyobfkd.sHtML

[Q85] 数值取整
来源：http://blog.zdbjq.cn/Article/details/gniuaqxtd.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.zdbjq.cn/Article/details/gthtvyywc.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fehbvm.com/Article/details/giyblgcyz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.zdbjq.cn/Article/details/gisyhknki.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.zdbjq.cn/Article/details/gtwgxgqbn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fehbvm.com/Article/details/gkxvyrhur.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fehbvm.com/Article/details/gussrmgls.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fehbvm.com/Article/details/gtpjbjgwx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fehbvm.com/Article/details/gnbcbkyac.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fehbvm.com/Article/details/geiiapwcw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.zdbjq.cn/Article/details/gujojmlot.sHtML

[Q90] 生成序号列
来源：http://baike.fehbvm.com/Article/details/gdzqlsrtm.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.hesvh.cn/Article/details/grneqqvdp.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gkypzxjtn.sHtML

R. Bash 专题
来源：http://baike.zdbjq.cn/Article/details/gqwroooha.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/giocllypw.sHtML

[R01] shebang 与严格模式
来源：http://blog.zdbjq.cn/Article/details/gyxczwnbe.sHtML

#!/usr/bin/env bash
来源：http://www.blog.hesvh.cn/Article/details/gnqxigxek.sHtML

set -euo pipefail
来源：http://mobile.fehbvm.com/Article/details/ghgznmxdw.sHtML

[R02] 变量赋值与使用
来源：http://read.share.zdbjq.cn/Article/details/gbblebjwg.sHtML

name="Tom"; echo "$name"
来源：http://mobile.zdbjq.cn/Article/details/gllqpywpx.sHtML

[R03] 只读变量
来源：http://3g.hesvh.cn/Article/details/ghdxokjgo.sHtML

readonly PI=3.14
来源：http://www.blog.zdbjq.cn/Article/details/grqbphtks.sHtML

[R04] 位置参数
来源：http://mobile.fehbvm.com/Article/details/gilrqhleu.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fehbvm.com/Article/details/gjjqzxjdo.sHtML

[R05] 参数默认值
来源：http://mobile.fehbvm.com/Article/details/gmukqkhdn.sHtML

name="${1:-default}"
来源：http://baike.zdbjq.cn/Article/details/gkuwmeiwh.sHtML

[R06] 判断命令是否存在
来源：http://mobile.zdbjq.cn/Article/details/ggrqbqtpf.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/geaeumhlt.sHtML

[R07] if 判断文件
来源：http://m.share.fehbvm.com/Article/details/gucbuknpb.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.hesvh.cn/Article/details/gywfssqzz.sHtML

[R08] 数值比较
来源：http://mobile.fehbvm.com/Article/details/gtytldjdu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.zdbjq.cn/Article/details/gtxmjetjs.sHtML

[R09] 字符串比较
来源：http://wap.hesvh.cn/Article/details/gxkuxanli.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fehbvm.com/Article/details/gadfdmjod.sHtML

[R10] 正则匹配
来源：http://blog.zdbjq.cn/Article/details/gzaxqdlbb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fehbvm.com/Article/details/gpcnbjttb.sHtML

[R11] case 多分支
来源：http://mobile.hesvh.cn/Article/details/gvpwclbaq.sHtML

case "$1" in
来源：http://read.share.zdbjq.cn/Article/details/gayrmrjnn.sHtML

start) echo "启动" ;;
来源：http://baike.zdbjq.cn/Article/details/gkhzxvytt.sHtML

stop)  echo "停止" ;;
来源：http://read.share.hesvh.cn/Article/details/gllvvoend.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fehbvm.com/Article/details/gtqqyutgr.sHtML

esac
来源：http://blog.hesvh.cn/Article/details/glzvpzeul.sHtML

[R12] for 遍历文件
来源：http://read.share.fehbvm.com/Article/details/ghrhypyru.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gfusdvmcs.sHtML

[R13] for 计数循环
来源：http://3g.fehbvm.com/Article/details/gwecwyhnw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/gupktdrrf.sHtML

[R14] C 风格 for
来源：http://3g.hesvh.cn/Article/details/gfpnuynuq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/ggrnkuieg.sHtML

[R15] while 逐行读文件
来源：http://3g.zdbjq.cn/Article/details/ggstytsln.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.zdbjq.cn/Article/details/ghmpjaesx.sHtML

[R16] until 等待条件
来源：http://m.share.fehbvm.com/Article/details/gynhcyxoh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gfspfvmxb.sHtML

[R17] 数组定义与取值
来源：http://mobile.fehbvm.com/Article/details/gwjclcvum.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fehbvm.com/Article/details/gudveqjnu.sHtML

[R18] 遍历数组
来源：http://wap.zdbjq.cn/Article/details/gbatnkcsv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fehbvm.com/Article/details/gshnhoufi.sHtML

[R19] 数组长度
来源：http://baike.fehbvm.com/Article/details/gdidwluhv.sHtML

echo "${#arr[@]}"
来源：http://www.share.fehbvm.com/Article/details/gviymtvir.sHtML

[R20] 关联数组（字典）
来源：http://read.share.zdbjq.cn/Article/details/guugfvxup.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.hesvh.cn/Article/details/gxsbxhshw.sHtML

[R21] 字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/guwlbteuj.sHtML

echo "${#s}"
来源：http://www.blog.fehbvm.com/Article/details/gcuzqvyfd.sHtML

[R22] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/gfutrdwzx.sHtML

echo "${s:0:5}"
来源：http://baike.zdbjq.cn/Article/details/gntdsuyrx.sHtML

[R23] 字符串替换
来源：http://blog.hesvh.cn/Article/details/gihugfgxk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.zdbjq.cn/Article/details/gguvpqspp.sHtML

[R24] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/gaobyozjx.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.hesvh.cn/Article/details/gaywwpceb.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.zdbjq.cn/Article/details/gofttqqoa.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.hesvh.cn/Article/details/gbaliiaqk.sHtML

[R26] 命令替换
来源：http://3g.fehbvm.com/Article/details/gzpgltrtl.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.hesvh.cn/Article/details/gzeoaztut.sHtML

[R27] 算术展开
来源：http://www.blog.hesvh.cn/Article/details/gmhkprccz.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fehbvm.com/Article/details/gyoplbhhy.sHtML

[R28] 浮点运算
来源：http://read.share.zdbjq.cn/Article/details/gjuxczcfb.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fehbvm.com/Article/details/gyuhuocgp.sHtML

[R29] 定义函数
来源：http://blog.fehbvm.com/Article/details/gxqaginbe.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fehbvm.com/Article/details/gudbzcjoq.sHtML

[R30] 函数返回状态码
来源：http://m.share.zdbjq.cn/Article/details/gbfozsfkg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.zdbjq.cn/Article/details/gtveczmvd.sHtML

[R31] 局部变量
来源：http://m.share.hesvh.cn/Article/details/gtvnlrxuw.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fehbvm.com/Article/details/gvqqvzncd.sHtML

[R32] 参数个数校验
来源：http://m.share.zdbjq.cn/Article/details/gwdjnzlho.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fehbvm.com/Article/details/gkjwgsfer.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fehbvm.com/Article/details/gswrumejh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.hesvh.cn/Article/details/grfsannvp.sHtML

[R34] 退出时清理
来源：http://blog.zdbjq.cn/Article/details/gggydyyzk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/ghvkjmmjv.sHtML

[R35] 后台执行并等待
来源：http://wap.zdbjq.cn/Article/details/gqlllkrrg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.hesvh.cn/Article/details/gmtfyaimi.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.zdbjq.cn/Article/details/gsxvxtjdu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.hesvh.cn/Article/details/gstvcfmbn.sHtML

[R37] 把输出赋给变量
来源：http://m.share.hesvh.cn/Article/details/gqmadkifn.sHtML

files=$(ls -1)
来源：http://wap.hesvh.cn/Article/details/gnfemibdt.sHtML

[R38] 管道串联
来源：http://baike.fehbvm.com/Article/details/gzyvaeays.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fehbvm.com/Article/details/glshhbozd.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.hesvh.cn/Article/details/ggovndhrf.sHtML

cmd > out.log 2>&1
来源：http://www.share.hesvh.cn/Article/details/gmizbgkpu.sHtML

[R40] 追加写日志
来源：http://read.share.fehbvm.com/Article/details/gypgmwzwq.sHtML

echo "log" >> out.log
来源：http://www.share.zdbjq.cn/Article/details/glcrreajw.sHtML

[R41] 丢弃输出
来源：http://www.blog.zdbjq.cn/Article/details/gzupebgvy.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gmsfvygna.sHtML

[R42] 输入重定向
来源：http://3g.fehbvm.com/Article/details/gmfvxxgmh.sHtML

wc -l < a.txt
来源：http://blog.fehbvm.com/Article/details/ghowicdph.sHtML

[R43] 按名字查找文件
来源：http://baike.hesvh.cn/Article/details/gtdlzssyz.sHtML

find . -name "*.log" -type f
来源：http://www.share.fehbvm.com/Article/details/gufubafnm.sHtML

[R44] 按修改时间查找
来源：http://wap.zdbjq.cn/Article/details/gofxxagwm.sHtML

find . -mtime -7 -type f
来源：http://3g.fehbvm.com/Article/details/gvdeehivw.sHtML

[R45] 批量删除
来源：http://www.share.zdbjq.cn/Article/details/gyjibghgg.sHtML

find . -name "*.tmp" -delete
来源：http://3g.hesvh.cn/Article/details/gktliwqoe.sHtML

[R46] 递归替换文件内容
来源：http://m.share.zdbjq.cn/Article/details/gdhoqcbhq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.hesvh.cn/Article/details/gdulsjpfe.sHtML

[R47] sed 单行替换
来源：http://blog.fehbvm.com/Article/details/gyuvqugvw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.hesvh.cn/Article/details/goplhzxla.sHtML

[R48] awk 取指定列
来源：http://m.share.hesvh.cn/Article/details/gzwbvhvxy.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gepvecjcc.sHtML

[R49] awk 带条件
来源：http://www.share.zdbjq.cn/Article/details/gjnnhloor.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.zdbjq.cn/Article/details/gefokmogv.sHtML

[R50] awk 求和
来源：http://blog.hesvh.cn/Article/details/ghspybavs.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fehbvm.com/Article/details/gdlcnioql.sHtML

[R51] 排序去重取前几
来源：http://wap.zdbjq.cn/Article/details/gddwygytc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.zdbjq.cn/Article/details/grvqurakz.sHtML

[R52] 统计行数
来源：http://blog.zdbjq.cn/Article/details/gogtkrjsk.sHtML

wc -l a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gccipotvp.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.zdbjq.cn/Article/details/gzerojvqh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fehbvm.com/Article/details/glbzrkzlt.sHtML

[R54] 比较两个文件
来源：http://wap.fehbvm.com/Article/details/gcjnbwdlb.sHtML

diff a.txt b.txt
来源：http://www.blog.zdbjq.cn/Article/details/gckmntvuz.sHtML

[R55] 压缩与解压
来源：http://m.share.fehbvm.com/Article/details/gmgtkmkej.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.zdbjq.cn/Article/details/gkcavhuav.sHtML

[R56] 远程拷贝
来源：http://m.share.hesvh.cn/Article/details/goffvhkdo.sHtML

scp file user@host:/path/
来源：http://baike.hesvh.cn/Article/details/gdwjwcdyo.sHtML

[R57] 远程执行命令
来源：http://blog.hesvh.cn/Article/details/gcwnbuisl.sHtML

ssh user@host 'uptime'
来源：http://baike.zdbjq.cn/Article/details/ginwbeeiz.sHtML

[R58] 下载文件
来源：http://mobile.hesvh.cn/Article/details/gyfhamprp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.zdbjq.cn/Article/details/gxdtxradq.sHtML

[R59] 发 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/gckizswgx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.hesvh.cn/Article/details/gsapennyb.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/gwbbudqrg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fehbvm.com/Article/details/gypmmrdfe.sHtML

[R61] 磁盘占用
来源：http://read.share.hesvh.cn/Article/details/gwanzfgbs.sHtML

df -h;  du -sh *
来源：http://www.blog.fehbvm.com/Article/details/gfxuuzlgn.sHtML

[R62] 找最占空间的文件
来源：http://3g.hesvh.cn/Article/details/gkndbscia.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.zdbjq.cn/Article/details/gfwzaayzw.sHtML

[R63] 内存与进程
来源：http://wap.zdbjq.cn/Article/details/gprszjmhg.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.hesvh.cn/Article/details/gwfkgavlr.sHtML

[R64] 结束进程
来源：http://m.share.fehbvm.com/Article/details/gpxfafyhl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fehbvm.com/Article/details/goigbkxvd.sHtML

[R65] 查看端口占用
来源：http://baike.fehbvm.com/Article/details/gymycsnjr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.zdbjq.cn/Article/details/gdgqsstie.sHtML

[R66] 定时任务
来源：http://www.m.share.hesvh.cn/Article/details/gqrjvykrz.sHtML

crontab -e;  crontab -l
来源：http://3g.fehbvm.com/Article/details/grwnycuqz.sHtML

[R67] 生成随机十六进制串
来源：http://baike.zdbjq.cn/Article/details/gwcuwqlnc.sHtML

openssl rand -hex 16
来源：http://www.m.share.hesvh.cn/Article/details/gaxwhiefr.sHtML

[R68] 计算文件校验值
来源：http://baike.fehbvm.com/Article/details/gzpccdmsh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gmmrphvqb.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fehbvm.com/Article/details/gqglwqrbe.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fehbvm.com/Article/details/gvdiujjyc.sHtML

[R70] 时间戳与互转
来源：http://read.share.fehbvm.com/Article/details/grxyqvdfi.sHtML

date +%s;  date -d @1700000000
来源：http://wap.zdbjq.cn/Article/details/gwoclmhjw.sHtML

[R71] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gzidixjwy.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.zdbjq.cn/Article/details/gtifvbadc.sHtML

[R72] 等待端口就绪
来源：http://3g.fehbvm.com/Article/details/gjqefcbfi.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/gbdxlkkji.sHtML

[R73] 分割大日志
来源：http://www.share.zdbjq.cn/Article/details/gjzgfdpzt.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fehbvm.com/Article/details/gakcmrzwa.sHtML

[R74] 批量重命名
来源：http://www.share.zdbjq.cn/Article/details/gqhfhngwz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fehbvm.com/Article/details/gpjsuidqo.sHtML

[R75] 导出环境变量
来源：http://mobile.hesvh.cn/Article/details/gdhqjfuwc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fehbvm.com/Article/details/gfhycdnmv.sHtML

[R76] 使用临时文件
来源：http://baike.fehbvm.com/Article/details/gtefqjrro.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gogxwdzpo.sHtML

[R77] 读取用户输入
来源：http://3g.hesvh.cn/Article/details/gbwmsnmii.sHtML

read -rp "请输入: " ans
来源：http://baike.hesvh.cn/Article/details/gmumudotc.sHtML

[R78] 交互式菜单
来源：http://m.share.hesvh.cn/Article/details/gmmwppfff.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.zdbjq.cn/Article/details/gkeibpmqe.sHtML

[R79] 解析命令行选项
来源：http://wap.zdbjq.cn/Article/details/gdpyjdmdu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.hesvh.cn/Article/details/gsagpjktl.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.zdbjq.cn/Article/details/gdadxyczj.sHtML

time ./run.sh
来源：http://wap.hesvh.cn/Article/details/gweqxalqb.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gbvunskzu.sHtML

S. C / C++ 专题
来源：http://mobile.fehbvm.com/Article/details/gtsmwlkfx.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gwvserayv.sHtML

[S01] C：Hello World
来源：http://blog.zdbjq.cn/Article/details/gfwzabzpo.sHtML

#include <stdio.h>
来源：http://www.share.hesvh.cn/Article/details/gmnmrcfqm.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fehbvm.com/Article/details/gfvmdcmod.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fehbvm.com/Article/details/geixhxilj.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fehbvm.com/Article/details/gxtjojntf.sHtML

[S03] C：读入整数
来源：http://baike.fehbvm.com/Article/details/gjdqqryot.sHtML

int x; scanf("%d", &x);
来源：http://m.share.zdbjq.cn/Article/details/gpwddjxbz.sHtML

[S04] C：字符串复制
来源：http://read.share.zdbjq.cn/Article/details/gefprspos.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.hesvh.cn/Article/details/gnigjtfwh.sHtML

[S05] C：字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gwalcczdr.sHtML

strlen(s)
来源：http://m.share.hesvh.cn/Article/details/gxkyuugdh.sHtML

[S06] C：字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/gmylkqqzz.sHtML

strcmp(a, b) == 0
来源：http://3g.fehbvm.com/Article/details/gfeguethc.sHtML

[S07] C：数组遍历求和
来源：http://3g.zdbjq.cn/Article/details/gvohsyjad.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.hesvh.cn/Article/details/gcdubdlcb.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fehbvm.com/Article/details/gagowowxk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.hesvh.cn/Article/details/gvmaoqcnk.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fehbvm.com/Article/details/gkkmzyejb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.hesvh.cn/Article/details/gklrjchpx.sHtML

[S10] C：指针与解引用
来源：http://3g.fehbvm.com/Article/details/glhmjeekx.sHtML

int *p = &a;  *p = 5;
来源：http://wap.hesvh.cn/Article/details/gdbykhzls.sHtML

[S11] C：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gnyikercq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.hesvh.cn/Article/details/gigdwglqd.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fehbvm.com/Article/details/gftzmimwn.sHtML

fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/gxqiusekv.sHtML

[S12] C：写文件
来源：http://baike.fehbvm.com/Article/details/gweeaavqw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.zdbjq.cn/Article/details/gfqaixarr.sHtML

[S13] C：宏定义
来源：http://www.blog.fehbvm.com/Article/details/grtgaqcym.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.zdbjq.cn/Article/details/gfxkwgemi.sHtML

[S14] C：枚举
来源：http://blog.hesvh.cn/Article/details/gojncvrjr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.hesvh.cn/Article/details/gyfemrkax.sHtML

[S15] C：类型转换
来源：http://mobile.hesvh.cn/Article/details/gqooygzbk.sHtML

(double) a / b
来源：http://wap.hesvh.cn/Article/details/gknzegxlc.sHtML

[S16] C：位操作置位
来源：http://blog.fehbvm.com/Article/details/gdehiebla.sHtML

x |= (1 << 3);
来源：http://mobile.fehbvm.com/Article/details/gbnvbezlf.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fehbvm.com/Article/details/gisqbszgc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fehbvm.com/Article/details/gjwgpiddh.sHtML

[S18] C：命令行参数
来源：http://www.blog.fehbvm.com/Article/details/gexcnenwc.sHtML

int main(int argc, char **argv)
来源：http://www.share.zdbjq.cn/Article/details/grwhhbtww.sHtML

[S19] C：快速排序
来源：http://wap.fehbvm.com/Article/details/gdaicrige.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gejsbhxmi.sHtML

[S20] C：二分查找
来源：http://m.share.zdbjq.cn/Article/details/gshzjjykl.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/golqdtakx.sHtML

[S21] C：字符类别判断
来源：http://www.share.fehbvm.com/Article/details/gahxhujey.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fehbvm.com/Article/details/galznwqgr.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fehbvm.com/Article/details/geoiooovs.sHtML


<!-- 参考信息 -->