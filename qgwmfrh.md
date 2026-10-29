代发 wailian999

[Q61] 移动平均
来源：http://baike.hesvh.cn/Article/details/gxxrkjnfd.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gfruhjjfm.sHtML

[Q62] 分组占比
来源：http://www.blog.zdbjq.cn/Article/details/giebttlgq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gajvbtsns.sHtML

[Q63] 开启事务
来源：http://m.share.hesvh.cn/Article/details/grymfwofu.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.hesvh.cn/Article/details/gphigrdme.sHtML

[Q64] 提交事务
来源：http://www.share.hesvh.cn/Article/details/grawriciq.sHtML

COMMIT;
来源：http://baike.hesvh.cn/Article/details/gpvkgncdb.sHtML

[Q65] 回滚事务
来源：http://read.share.fehbvm.com/Article/details/gpvmtxsvg.sHtML

ROLLBACK;
来源：http://blog.zdbjq.cn/Article/details/gbsdopjdn.sHtML

[Q66] 行锁查询
来源：http://read.share.hesvh.cn/Article/details/gnitjkniq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fehbvm.com/Article/details/goswetlrw.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fehbvm.com/Article/details/gfnweafsy.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fehbvm.com/Article/details/gomviuimb.sHtML

[Q68] 保存点
来源：http://read.share.fehbvm.com/Article/details/gbyuvpgle.sHtML

SAVEPOINT sp1;
来源：http://wap.hesvh.cn/Article/details/grcuxwmrg.sHtML

ROLLBACK TO sp1;
来源：http://m.share.zdbjq.cn/Article/details/gxkspspkn.sHtML

[Q69] 查看执行计划
来源：http://www.blog.zdbjq.cn/Article/details/gyulmbupm.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fehbvm.com/Article/details/gecrlouko.sHtML

[Q70] 更新统计信息
来源：http://mobile.zdbjq.cn/Article/details/goyjnqwir.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.zdbjq.cn/Article/details/gtydbuyag.sHtML

[Q71] 查看建表语句
来源：http://3g.hesvh.cn/Article/details/gxepuewip.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.fehbvm.com/Article/details/gjetlhish.sHtML

[Q72] 查看索引
来源：http://baike.fehbvm.com/Article/details/gzdqqnulz.sHtML

SHOW INDEX FROM users;
来源：http://3g.hesvh.cn/Article/details/gcuwkmibv.sHtML

[Q73] 查看表状态
来源：http://3g.fehbvm.com/Article/details/gyjmujjqn.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.hesvh.cn/Article/details/gpcqbdgro.sHtML

[Q74] 强制使用索引
来源：http://www.blog.zdbjq.cn/Article/details/gnezrpagc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fehbvm.com/Article/details/gxtyxikpd.sHtML

[Q75] 日期格式化
来源：http://baike.hesvh.cn/Article/details/guuzrffos.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gshotkspt.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.hesvh.cn/Article/details/gncfoohmh.sHtML

[Q76] 按天统计
来源：http://www.m.share.zdbjq.cn/Article/details/gcmtfopmn.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.hesvh.cn/Article/details/gcbbujogo.sHtML

[Q77] 时间加减
来源：http://baike.fehbvm.com/Article/details/gldwmtnhu.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.zdbjq.cn/Article/details/grymrssaw.sHtML

[Q78] 当前时间
来源：http://www.m.share.fehbvm.com/Article/details/gectyembr.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fehbvm.com/Article/details/gpfvnncvv.sHtML

[Q79] 字符串拼接
来源：http://mobile.zdbjq.cn/Article/details/gdnjkcttk.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.hesvh.cn/Article/details/gbvwundip.sHtML

[Q80] 字符串截取
来源：http://read.share.hesvh.cn/Article/details/gnzbohake.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gxpdagalz.sHtML

[Q81] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gsaarsiqh.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gnetfpgba.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.hesvh.cn/Article/details/gqbgrnnri.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gmkmkiqiw.sHtML

[Q83] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gssfisyhg.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gnvhfdyky.sHtML

[Q84] 去除首尾空格
来源：http://3g.zdbjq.cn/Article/details/gkzroarwq.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gpqjcyzeo.sHtML

[Q85] 数值取整
来源：http://wap.zdbjq.cn/Article/details/gzuverjag.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fehbvm.com/Article/details/gnsjzockb.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.hesvh.cn/Article/details/gomeeqcqt.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fehbvm.com/Article/details/glpmvalti.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fehbvm.com/Article/details/gomlebkns.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.zdbjq.cn/Article/details/gwrtleijs.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.zdbjq.cn/Article/details/gceeqynwc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.hesvh.cn/Article/details/ghctwvsob.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.zdbjq.cn/Article/details/gkxgwjzyb.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fehbvm.com/Article/details/gyrmzuwev.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.hesvh.cn/Article/details/gxdnymqnr.sHtML

[Q90] 生成序号列
来源：http://3g.zdbjq.cn/Article/details/gikxmqwmn.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fehbvm.com/Article/details/gbjwwpdpl.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gjiizwdmf.sHtML

R. Bash 专题
来源：http://www.blog.zdbjq.cn/Article/details/ghcdlqdhy.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gxxvtifbq.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.zdbjq.cn/Article/details/gslkwmncu.sHtML

#!/usr/bin/env bash
来源：http://read.share.zdbjq.cn/Article/details/gvgigswks.sHtML

set -euo pipefail
来源：http://wap.fehbvm.com/Article/details/guutgyzln.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fehbvm.com/Article/details/gcsfdcbje.sHtML

name="Tom"; echo "$name"
来源：http://3g.hesvh.cn/Article/details/gpjailwew.sHtML

[R03] 只读变量
来源：http://read.share.fehbvm.com/Article/details/gqonllrjq.sHtML

readonly PI=3.14
来源：http://www.blog.fehbvm.com/Article/details/gzniclywi.sHtML

[R04] 位置参数
来源：http://mobile.zdbjq.cn/Article/details/ghmmakhiz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.hesvh.cn/Article/details/gaspagidq.sHtML

[R05] 参数默认值
来源：http://baike.fehbvm.com/Article/details/ghqthxbow.sHtML

name="${1:-default}"
来源：http://blog.fehbvm.com/Article/details/gabucjdvd.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fehbvm.com/Article/details/giauceeca.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/gokqowvqt.sHtML

[R07] if 判断文件
来源：http://www.blog.fehbvm.com/Article/details/gazljkvxw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.zdbjq.cn/Article/details/gfaykgxtv.sHtML

[R08] 数值比较
来源：http://blog.hesvh.cn/Article/details/gehniyyrz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.hesvh.cn/Article/details/gmjsjafyo.sHtML

[R09] 字符串比较
来源：http://blog.hesvh.cn/Article/details/gjotpmqkz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.zdbjq.cn/Article/details/ggkayqojj.sHtML

[R10] 正则匹配
来源：http://www.m.share.hesvh.cn/Article/details/gcsekqxcb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.hesvh.cn/Article/details/glskvstcj.sHtML

[R11] case 多分支
来源：http://read.share.fehbvm.com/Article/details/getaynbbp.sHtML

case "$1" in
来源：http://read.share.fehbvm.com/Article/details/gtusgvvop.sHtML

start) echo "启动" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/guopoanqu.sHtML

stop)  echo "停止" ;;
来源：http://read.share.zdbjq.cn/Article/details/gazdqdula.sHtML

*)     echo "未知命令" ;;
来源：http://wap.hesvh.cn/Article/details/gpfstwycw.sHtML

esac
来源：http://www.share.zdbjq.cn/Article/details/gwhllqlxz.sHtML

[R12] for 遍历文件
来源：http://mobile.hesvh.cn/Article/details/gomqxhigk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.hesvh.cn/Article/details/ghjgeliei.sHtML

[R13] for 计数循环
来源：http://wap.zdbjq.cn/Article/details/ghacpbonk.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/gqgpxkxmm.sHtML

[R14] C 风格 for
来源：http://wap.zdbjq.cn/Article/details/ghmbssdgc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gyeztcuhn.sHtML

[R15] while 逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gxmzhfyxv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fehbvm.com/Article/details/gnnneykcy.sHtML

[R16] until 等待条件
来源：http://3g.hesvh.cn/Article/details/gaumadpzz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/gffdklonp.sHtML

[R17] 数组定义与取值
来源：http://read.share.fehbvm.com/Article/details/ggariziac.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fehbvm.com/Article/details/gnducdpnc.sHtML

[R18] 遍历数组
来源：http://www.share.hesvh.cn/Article/details/gkcifjnqb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fehbvm.com/Article/details/gxhhecsvk.sHtML

[R19] 数组长度
来源：http://baike.fehbvm.com/Article/details/grnwfywet.sHtML

echo "${#arr[@]}"
来源：http://m.share.hesvh.cn/Article/details/gablgqhjr.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fehbvm.com/Article/details/gydrbpgcs.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.zdbjq.cn/Article/details/gnzfchlqy.sHtML

[R21] 字符串长度
来源：http://wap.zdbjq.cn/Article/details/givlwpdac.sHtML

echo "${#s}"
来源：http://read.share.hesvh.cn/Article/details/gboobsyrf.sHtML

[R22] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/gqmljzecn.sHtML

echo "${s:0:5}"
来源：http://www.share.fehbvm.com/Article/details/gklyoqvni.sHtML

[R23] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/gubuwrguy.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.hesvh.cn/Article/details/gzevpglle.sHtML

[R24] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/gldylaihr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fehbvm.com/Article/details/ghlixbyev.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.hesvh.cn/Article/details/gxelvclrl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fehbvm.com/Article/details/gjvneduax.sHtML

[R26] 命令替换
来源：http://baike.hesvh.cn/Article/details/gjukzpegf.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.hesvh.cn/Article/details/gtvuwadwh.sHtML

[R27] 算术展开
来源：http://3g.zdbjq.cn/Article/details/gmviniskz.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fehbvm.com/Article/details/ghdcoxgnc.sHtML

[R28] 浮点运算
来源：http://www.share.fehbvm.com/Article/details/guvzbrlrk.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.hesvh.cn/Article/details/giujxesoi.sHtML

[R29] 定义函数
来源：http://blog.hesvh.cn/Article/details/ghwjxocby.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.hesvh.cn/Article/details/gvzkiuodg.sHtML

[R30] 函数返回状态码
来源：http://blog.fehbvm.com/Article/details/gfvqqdtho.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fehbvm.com/Article/details/gxdjsgcsb.sHtML

[R31] 局部变量
来源：http://mobile.zdbjq.cn/Article/details/gotzoqmwm.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fehbvm.com/Article/details/gqwdnblte.sHtML

[R32] 参数个数校验
来源：http://mobile.zdbjq.cn/Article/details/gswghtpca.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/gqclnpumd.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.zdbjq.cn/Article/details/gltgyidhp.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.zdbjq.cn/Article/details/gdogmelna.sHtML

[R34] 退出时清理
来源：http://baike.fehbvm.com/Article/details/gjuzgsson.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/gtajjolax.sHtML

[R35] 后台执行并等待
来源：http://mobile.fehbvm.com/Article/details/grrejfqou.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.zdbjq.cn/Article/details/gazcevybk.sHtML

[R36] 并发执行多个任务
来源：http://www.share.hesvh.cn/Article/details/gcexkferx.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.hesvh.cn/Article/details/gjadwioel.sHtML

[R37] 把输出赋给变量
来源：http://read.share.zdbjq.cn/Article/details/gglgvkvxg.sHtML

files=$(ls -1)
来源：http://3g.zdbjq.cn/Article/details/gmhroivhd.sHtML

[R38] 管道串联
来源：http://www.share.fehbvm.com/Article/details/ggfxyzuci.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.hesvh.cn/Article/details/gfjzmkvrw.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.zdbjq.cn/Article/details/grrvxyxgm.sHtML

cmd > out.log 2>&1
来源：http://read.share.fehbvm.com/Article/details/gzoutpiqe.sHtML

[R40] 追加写日志
来源：http://read.share.fehbvm.com/Article/details/gkrzrwpes.sHtML

echo "log" >> out.log
来源：http://www.share.zdbjq.cn/Article/details/glckznwut.sHtML

[R41] 丢弃输出
来源：http://wap.fehbvm.com/Article/details/gzgrrrgrx.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fehbvm.com/Article/details/ghtnnjcrr.sHtML

[R42] 输入重定向
来源：http://wap.hesvh.cn/Article/details/gevsjrhny.sHtML

wc -l < a.txt
来源：http://wap.fehbvm.com/Article/details/gkuicqsyx.sHtML

[R43] 按名字查找文件
来源：http://3g.fehbvm.com/Article/details/gbqyejscl.sHtML

find . -name "*.log" -type f
来源：http://blog.hesvh.cn/Article/details/gdtewgjuj.sHtML

[R44] 按修改时间查找
来源：http://www.share.zdbjq.cn/Article/details/guqkbyeru.sHtML

find . -mtime -7 -type f
来源：http://baike.zdbjq.cn/Article/details/gukabekyp.sHtML

[R45] 批量删除
来源：http://read.share.hesvh.cn/Article/details/gauynhmrs.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.hesvh.cn/Article/details/gcxmcdqtm.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fehbvm.com/Article/details/gitimvruz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.hesvh.cn/Article/details/gdirfendl.sHtML

[R47] sed 单行替换
来源：http://www.m.share.hesvh.cn/Article/details/gownhacjj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gwyfzmrhl.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fehbvm.com/Article/details/gauxakjrx.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fehbvm.com/Article/details/gmbqmqgrd.sHtML

[R49] awk 带条件
来源：http://blog.zdbjq.cn/Article/details/gcwzmockl.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.hesvh.cn/Article/details/gpocoambw.sHtML

[R50] awk 求和
来源：http://mobile.hesvh.cn/Article/details/gqjxrutjw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gtznmrwkh.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fehbvm.com/Article/details/gskhsbvdb.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.zdbjq.cn/Article/details/gvtzcahjv.sHtML

[R52] 统计行数
来源：http://baike.hesvh.cn/Article/details/gzlxnqvmv.sHtML

wc -l a.txt
来源：http://www.blog.hesvh.cn/Article/details/gfcnyzlfc.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.hesvh.cn/Article/details/gpyvivddg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.zdbjq.cn/Article/details/gbrrunqnc.sHtML

[R54] 比较两个文件
来源：http://mobile.fehbvm.com/Article/details/gqlfhykww.sHtML

diff a.txt b.txt
来源：http://www.blog.zdbjq.cn/Article/details/genpfapuu.sHtML

[R55] 压缩与解压
来源：http://baike.zdbjq.cn/Article/details/gqkwaoypq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.zdbjq.cn/Article/details/gkicjxykb.sHtML

[R56] 远程拷贝
来源：http://www.blog.hesvh.cn/Article/details/glllyhsyu.sHtML

scp file user@host:/path/
来源：http://mobile.zdbjq.cn/Article/details/gdilnqrfb.sHtML

[R57] 远程执行命令
来源：http://www.blog.fehbvm.com/Article/details/gchzorsjb.sHtML

ssh user@host 'uptime'
来源：http://www.share.fehbvm.com/Article/details/gynedcuhk.sHtML

[R58] 下载文件
来源：http://blog.hesvh.cn/Article/details/gvpglepyn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.hesvh.cn/Article/details/gneeomfdv.sHtML

[R59] 发 POST JSON
来源：http://www.share.fehbvm.com/Article/details/gqcytethw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.hesvh.cn/Article/details/glfpwtvoz.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/goziuflrz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.hesvh.cn/Article/details/grzzfubok.sHtML

[R61] 磁盘占用
来源：http://www.share.hesvh.cn/Article/details/gevxqdthr.sHtML

df -h;  du -sh *
来源：http://baike.hesvh.cn/Article/details/gvkruzehe.sHtML

[R62] 找最占空间的文件
来源：http://mobile.hesvh.cn/Article/details/ghlrkdqhv.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.zdbjq.cn/Article/details/goriextux.sHtML

[R63] 内存与进程
来源：http://3g.hesvh.cn/Article/details/grdztlqmi.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.zdbjq.cn/Article/details/gbpmwamgk.sHtML

[R64] 结束进程
来源：http://mobile.hesvh.cn/Article/details/geaswlpul.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.zdbjq.cn/Article/details/glyvotsbm.sHtML

[R65] 查看端口占用
来源：http://www.blog.hesvh.cn/Article/details/gmyjkdpdf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fehbvm.com/Article/details/gxlhkwdmf.sHtML

[R66] 定时任务
来源：http://baike.zdbjq.cn/Article/details/ghxudrqkl.sHtML

crontab -e;  crontab -l
来源：http://read.share.fehbvm.com/Article/details/gsxwwllbn.sHtML

[R67] 生成随机十六进制串
来源：http://blog.zdbjq.cn/Article/details/gdtaophhm.sHtML

openssl rand -hex 16
来源：http://read.share.hesvh.cn/Article/details/gzhonexhl.sHtML

[R68] 计算文件校验值
来源：http://3g.fehbvm.com/Article/details/guhuwzugp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gtywfakts.sHtML

[R69] 生成随机密码
来源：http://www.share.zdbjq.cn/Article/details/gdqkwwaxi.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.hesvh.cn/Article/details/gckswnnlq.sHtML

[R70] 时间戳与互转
来源：http://3g.hesvh.cn/Article/details/gtqutboay.sHtML

date +%s;  date -d @1700000000
来源：http://baike.hesvh.cn/Article/details/gvbeocscs.sHtML

[R71] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gopmloyks.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.zdbjq.cn/Article/details/gzpbolqmg.sHtML

[R72] 等待端口就绪
来源：http://baike.fehbvm.com/Article/details/gknciowma.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/gipfwixhv.sHtML

[R73] 分割大日志
来源：http://m.share.fehbvm.com/Article/details/ghyhmdyxj.sHtML

split -l 1000 big.log part_
来源：http://blog.hesvh.cn/Article/details/gcocanzwt.sHtML

[R74] 批量重命名
来源：http://wap.fehbvm.com/Article/details/guofgczxb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.hesvh.cn/Article/details/gmvfvduwc.sHtML

[R75] 导出环境变量
来源：http://3g.fehbvm.com/Article/details/grgrwncee.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.zdbjq.cn/Article/details/goerohkkd.sHtML

[R76] 使用临时文件
来源：http://m.share.fehbvm.com/Article/details/gwztzpjna.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gzgzxmktr.sHtML

[R77] 读取用户输入
来源：http://3g.fehbvm.com/Article/details/gpjghzhzk.sHtML

read -rp "请输入: " ans
来源：http://read.share.zdbjq.cn/Article/details/gbsqjtyic.sHtML

[R78] 交互式菜单
来源：http://baike.fehbvm.com/Article/details/gwajmwqtp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fehbvm.com/Article/details/gzfikvtcs.sHtML

[R79] 解析命令行选项
来源：http://mobile.zdbjq.cn/Article/details/gffmrmeoi.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fehbvm.com/Article/details/gsoczdaac.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.hesvh.cn/Article/details/gdfjhkffa.sHtML

time ./run.sh
来源：http://3g.hesvh.cn/Article/details/gkvbgyfuq.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gpwppnipq.sHtML

S. C / C++ 专题
来源：http://blog.fehbvm.com/Article/details/gzgdgknqi.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gsgxzkclu.sHtML

[S01] C：Hello World
来源：http://mobile.hesvh.cn/Article/details/grtxgppzx.sHtML

#include <stdio.h>
来源：http://baike.zdbjq.cn/Article/details/ggtuyyxhb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fehbvm.com/Article/details/gfarwdqgq.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fehbvm.com/Article/details/gmvikyscx.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.zdbjq.cn/Article/details/gmwfthamg.sHtML

[S03] C：读入整数
来源：http://mobile.hesvh.cn/Article/details/gxfszhyuw.sHtML

int x; scanf("%d", &x);
来源：http://blog.hesvh.cn/Article/details/gjjbrbxab.sHtML

[S04] C：字符串复制
来源：http://mobile.zdbjq.cn/Article/details/gmnpldpsu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fehbvm.com/Article/details/gztlubpfo.sHtML

[S05] C：字符串长度
来源：http://blog.hesvh.cn/Article/details/gkvhuhhfe.sHtML

strlen(s)
来源：http://www.m.share.hesvh.cn/Article/details/gkujavgdb.sHtML

[S06] C：字符串比较
来源：http://baike.fehbvm.com/Article/details/gvoimepau.sHtML

strcmp(a, b) == 0
来源：http://wap.hesvh.cn/Article/details/gdjmaxmfm.sHtML

[S07] C：数组遍历求和
来源：http://mobile.zdbjq.cn/Article/details/gipjewiwq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.zdbjq.cn/Article/details/gzuhehtrb.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.zdbjq.cn/Article/details/gobvppapi.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.zdbjq.cn/Article/details/gjsgxnexo.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.hesvh.cn/Article/details/gztsmhjkb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.zdbjq.cn/Article/details/ghzrnseco.sHtML

[S10] C：指针与解引用
来源：http://wap.zdbjq.cn/Article/details/gzfxokpvm.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.hesvh.cn/Article/details/gtlmymkrv.sHtML

[S11] C：逐行读文件
来源：http://blog.fehbvm.com/Article/details/guhkdhxxu.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.hesvh.cn/Article/details/gczggdbul.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gdexagztb.sHtML

fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gebgzmqae.sHtML

[S12] C：写文件
来源：http://m.share.zdbjq.cn/Article/details/gptgiqoox.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fehbvm.com/Article/details/gsctzqakj.sHtML

[S13] C：宏定义
来源：http://www.m.share.fehbvm.com/Article/details/gtfkqryum.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.zdbjq.cn/Article/details/gwcjzyamm.sHtML

[S14] C：枚举
来源：http://mobile.zdbjq.cn/Article/details/gkkstfclf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.zdbjq.cn/Article/details/gcszhmvpv.sHtML

[S15] C：类型转换
来源：http://m.share.zdbjq.cn/Article/details/gxengsged.sHtML

(double) a / b
来源：http://baike.zdbjq.cn/Article/details/gzznxeesh.sHtML

[S16] C：位操作置位
来源：http://3g.zdbjq.cn/Article/details/gqucsoeud.sHtML

x |= (1 << 3);
来源：http://wap.fehbvm.com/Article/details/ggyvogpho.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gmnapbljt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.zdbjq.cn/Article/details/glhhqknkm.sHtML

[S18] C：命令行参数
来源：http://read.share.hesvh.cn/Article/details/gvmlfvxgq.sHtML

int main(int argc, char **argv)
来源：http://read.share.fehbvm.com/Article/details/gxnehedxb.sHtML

[S19] C：快速排序
来源：http://www.blog.zdbjq.cn/Article/details/gfngudyth.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/gptmxbwbe.sHtML

[S20] C：二分查找
来源：http://www.m.share.fehbvm.com/Article/details/gsfhcflag.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/gqrlfthsw.sHtML

[S21] C：字符类别判断
来源：http://www.blog.zdbjq.cn/Article/details/gdxmfuibp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fehbvm.com/Article/details/gnkqhycjp.sHtML

[S22] C：字符串转数字
来源：http://3g.hesvh.cn/Article/details/gptdmprpp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.zdbjq.cn/Article/details/gxsswkgxi.sHtML

[S23] C：随机数
来源：http://www.blog.zdbjq.cn/Article/details/gtqsdfnjt.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.zdbjq.cn/Article/details/grtsgxqmd.sHtML

[S24] C：获取本地时间
来源：http://3g.fehbvm.com/Article/details/gctprxthf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.hesvh.cn/Article/details/gwhwwksic.sHtML

[S25] C：内存拷贝
来源：http://www.share.fehbvm.com/Article/details/gzxsvbcee.sHtML

memcpy(dst, src, n);
来源：http://mobile.hesvh.cn/Article/details/gvolibhgt.sHtML

[S26] C：内存清零
来源：http://www.share.fehbvm.com/Article/details/grsljixxf.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.hesvh.cn/Article/details/gexhalsfr.sHtML

[S27] C：定义常量
来源：http://www.share.hesvh.cn/Article/details/gyntdnpor.sHtML

const double PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gblrmpvih.sHtML

[S28] C：静态变量
来源：http://3g.fehbvm.com/Article/details/gxwzhlqgp.sHtML

static int counter = 0;
来源：http://read.share.hesvh.cn/Article/details/gppevrvtl.sHtML

[S29] C：变参函数
来源：http://mobile.zdbjq.cn/Article/details/gpisbckoc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fehbvm.com/Article/details/grtpfmjag.sHtML

[S30] C：头文件保护
来源：http://www.m.share.zdbjq.cn/Article/details/ggtforzgi.sHtML

#ifndef X_H
来源：http://3g.zdbjq.cn/Article/details/gucowwcwo.sHtML

#define X_H
来源：http://3g.zdbjq.cn/Article/details/gdfluosss.sHtML

#endif
来源：http://baike.fehbvm.com/Article/details/gatgugdlu.sHtML

[S31] C++：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gbyrvkcng.sHtML


<!-- 参考信息 -->