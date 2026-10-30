代发 wailian999

SHOW INDEX FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gyzztkeiw.sHtML

[Q73] 查看表状态
来源：http://read.share.zdbjq.cn/Article/details/gjazfmnpd.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.zdbjq.cn/Article/details/gzlgzegig.sHtML

[Q74] 强制使用索引
来源：http://www.blog.hesvh.cn/Article/details/gbifvqwbq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.zdbjq.cn/Article/details/gtaokdldd.sHtML

[Q75] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gfohnqqvl.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fehbvm.com/Article/details/gxtonxhgz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fehbvm.com/Article/details/gfphawycs.sHtML

[Q76] 按天统计
来源：http://3g.fehbvm.com/Article/details/gnbtewvnk.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.zdbjq.cn/Article/details/gejurhjzv.sHtML

[Q77] 时间加减
来源：http://wap.fehbvm.com/Article/details/gasgrbczt.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.zdbjq.cn/Article/details/gljozwwlp.sHtML

[Q78] 当前时间
来源：http://www.blog.hesvh.cn/Article/details/golbyjhdk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.hesvh.cn/Article/details/gzonekxzt.sHtML

[Q79] 字符串拼接
来源：http://wap.hesvh.cn/Article/details/gvkbcscac.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.hesvh.cn/Article/details/gvrahiqau.sHtML

[Q80] 字符串截取
来源：http://mobile.hesvh.cn/Article/details/gkuhkmoeg.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.hesvh.cn/Article/details/gigznimar.sHtML

[Q81] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/gfwjnmdyv.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gcmkzbwyd.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.zdbjq.cn/Article/details/gaehxknqn.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gaswtkskx.sHtML

[Q83] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/ggnrqafdn.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gfxqqtgnd.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fehbvm.com/Article/details/gtkgrsllw.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gjkqwjqfu.sHtML

[Q85] 数值取整
来源：http://3g.hesvh.cn/Article/details/gixfclznn.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.zdbjq.cn/Article/details/gryjdijpm.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.zdbjq.cn/Article/details/gecquqfxh.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.zdbjq.cn/Article/details/gqfmmivqm.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fehbvm.com/Article/details/gciugklge.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fehbvm.com/Article/details/gqnbkbley.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.hesvh.cn/Article/details/gohlbzgxk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.hesvh.cn/Article/details/goqhkfncj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fehbvm.com/Article/details/gbbxuahju.sHtML

[Q89] 判断表是否存在
来源：http://read.share.zdbjq.cn/Article/details/gtdzmgzwg.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fehbvm.com/Article/details/gogfeajyl.sHtML

[Q90] 生成序号列
来源：http://www.share.fehbvm.com/Article/details/gbgqyzzrs.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fehbvm.com/Article/details/gxhvuloou.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gpmxfccep.sHtML

R. Bash 专题
来源：http://mobile.zdbjq.cn/Article/details/gvetwokwq.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gxqaiuryo.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fehbvm.com/Article/details/gflkjhjuh.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.hesvh.cn/Article/details/gvwpjvlcp.sHtML

set -euo pipefail
来源：http://www.share.zdbjq.cn/Article/details/gdylbfxlt.sHtML

[R02] 变量赋值与使用
来源：http://baike.zdbjq.cn/Article/details/gjtayitmp.sHtML

name="Tom"; echo "$name"
来源：http://read.share.hesvh.cn/Article/details/gzxzkfyxi.sHtML

[R03] 只读变量
来源：http://3g.hesvh.cn/Article/details/gfpwtfxhx.sHtML

readonly PI=3.14
来源：http://wap.fehbvm.com/Article/details/gikkzbhcd.sHtML

[R04] 位置参数
来源：http://www.m.share.fehbvm.com/Article/details/gahcqqpym.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.hesvh.cn/Article/details/genyjeqce.sHtML

[R05] 参数默认值
来源：http://www.share.hesvh.cn/Article/details/gbfnioyia.sHtML

name="${1:-default}"
来源：http://blog.fehbvm.com/Article/details/gwtmrpyeb.sHtML

[R06] 判断命令是否存在
来源：http://blog.fehbvm.com/Article/details/gpdjdhlls.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/gijsqywkr.sHtML

[R07] if 判断文件
来源：http://m.share.hesvh.cn/Article/details/gqmtbgvgf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.hesvh.cn/Article/details/gmznpygxa.sHtML

[R08] 数值比较
来源：http://www.blog.fehbvm.com/Article/details/gdooswzfd.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.zdbjq.cn/Article/details/geygduank.sHtML

[R09] 字符串比较
来源：http://wap.hesvh.cn/Article/details/gonhelmpf.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.zdbjq.cn/Article/details/gnslbstre.sHtML

[R10] 正则匹配
来源：http://wap.zdbjq.cn/Article/details/gonbzrqql.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gyhilcorg.sHtML

[R11] case 多分支
来源：http://read.share.fehbvm.com/Article/details/gqnttihfw.sHtML

case "$1" in
来源：http://baike.hesvh.cn/Article/details/gyxtrvbrs.sHtML

start) echo "启动" ;;
来源：http://www.blog.fehbvm.com/Article/details/gtjailpto.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fehbvm.com/Article/details/gzllsftbi.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.hesvh.cn/Article/details/gfxwotznh.sHtML

esac
来源：http://www.share.hesvh.cn/Article/details/gmeiphclk.sHtML

[R12] for 遍历文件
来源：http://www.blog.zdbjq.cn/Article/details/ghagdlgom.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.zdbjq.cn/Article/details/gxoqhzvgl.sHtML

[R13] for 计数循环
来源：http://mobile.zdbjq.cn/Article/details/gcyixtits.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/ghzbvzbly.sHtML

[R14] C 风格 for
来源：http://mobile.hesvh.cn/Article/details/gueayhdth.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/gmdjfbcli.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gqrbiknvr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.hesvh.cn/Article/details/ghkeymrgf.sHtML

[R16] until 等待条件
来源：http://www.m.share.fehbvm.com/Article/details/gwfjiknzk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/gecgcatyl.sHtML

[R17] 数组定义与取值
来源：http://m.share.fehbvm.com/Article/details/gyjrwwkcb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.zdbjq.cn/Article/details/gdevlvbmd.sHtML

[R18] 遍历数组
来源：http://3g.fehbvm.com/Article/details/gxgzryguw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fehbvm.com/Article/details/gfpmozgfl.sHtML

[R19] 数组长度
来源：http://wap.zdbjq.cn/Article/details/gccvecppl.sHtML

echo "${#arr[@]}"
来源：http://mobile.fehbvm.com/Article/details/gvaupqldp.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.zdbjq.cn/Article/details/gccblaejk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fehbvm.com/Article/details/gvpvyulyg.sHtML

[R21] 字符串长度
来源：http://blog.fehbvm.com/Article/details/ghoquifff.sHtML

echo "${#s}"
来源：http://m.share.hesvh.cn/Article/details/geaagdsqr.sHtML

[R22] 截取子串
来源：http://3g.hesvh.cn/Article/details/gwelxyuyc.sHtML

echo "${s:0:5}"
来源：http://baike.hesvh.cn/Article/details/giujclomp.sHtML

[R23] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/gcczlpohn.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.hesvh.cn/Article/details/gjfnynawn.sHtML

[R24] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gmgvcnfqx.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fehbvm.com/Article/details/gmpgbwfcw.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.hesvh.cn/Article/details/gjgthdzsy.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fehbvm.com/Article/details/ghdqtqbvf.sHtML

[R26] 命令替换
来源：http://www.share.fehbvm.com/Article/details/grkikyxab.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fehbvm.com/Article/details/gklybduyh.sHtML

[R27] 算术展开
来源：http://read.share.fehbvm.com/Article/details/ghcocwvyv.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fehbvm.com/Article/details/gssaalnyy.sHtML

[R28] 浮点运算
来源：http://blog.zdbjq.cn/Article/details/gkfjnbqpm.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fehbvm.com/Article/details/gxbkvjvns.sHtML

[R29] 定义函数
来源：http://www.share.hesvh.cn/Article/details/gqijxxlpf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.hesvh.cn/Article/details/ghhudgzsg.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gfzcyolen.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fehbvm.com/Article/details/ggcppiitt.sHtML

[R31] 局部变量
来源：http://mobile.fehbvm.com/Article/details/guasyuhga.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fehbvm.com/Article/details/gosaszksa.sHtML

[R32] 参数个数校验
来源：http://blog.hesvh.cn/Article/details/gibpthltt.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/gqkojwlct.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.zdbjq.cn/Article/details/gatwlcizo.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.hesvh.cn/Article/details/groukevjh.sHtML

[R34] 退出时清理
来源：http://www.m.share.hesvh.cn/Article/details/gwxlplzxm.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gsilakgwh.sHtML

[R35] 后台执行并等待
来源：http://blog.fehbvm.com/Article/details/gldwaebtl.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.zdbjq.cn/Article/details/gdrhfcpqe.sHtML

[R36] 并发执行多个任务
来源：http://3g.hesvh.cn/Article/details/gogmirhrp.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fehbvm.com/Article/details/gcopzxvze.sHtML

[R37] 把输出赋给变量
来源：http://read.share.hesvh.cn/Article/details/gpcwsgyzx.sHtML

files=$(ls -1)
来源：http://mobile.fehbvm.com/Article/details/gjgajgfqb.sHtML

[R38] 管道串联
来源：http://read.share.hesvh.cn/Article/details/gosknhqeb.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.hesvh.cn/Article/details/gkocdzvpw.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fehbvm.com/Article/details/gndlmucib.sHtML

cmd > out.log 2>&1
来源：http://baike.zdbjq.cn/Article/details/gbugbzmvs.sHtML

[R40] 追加写日志
来源：http://read.share.zdbjq.cn/Article/details/ghrcptfmx.sHtML

echo "log" >> out.log
来源：http://baike.hesvh.cn/Article/details/gfomeiwhl.sHtML

[R41] 丢弃输出
来源：http://www.blog.zdbjq.cn/Article/details/gamkkshgj.sHtML

cmd >/dev/null 2>&1
来源：http://wap.hesvh.cn/Article/details/gcicbzqmt.sHtML

[R42] 输入重定向
来源：http://mobile.hesvh.cn/Article/details/gtkfchfmp.sHtML

wc -l < a.txt
来源：http://www.share.zdbjq.cn/Article/details/gefnydqlr.sHtML

[R43] 按名字查找文件
来源：http://mobile.fehbvm.com/Article/details/gacncewpj.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.zdbjq.cn/Article/details/gqgszkief.sHtML

[R44] 按修改时间查找
来源：http://wap.fehbvm.com/Article/details/gdfkesqro.sHtML

find . -mtime -7 -type f
来源：http://mobile.fehbvm.com/Article/details/gomsrsmis.sHtML

[R45] 批量删除
来源：http://read.share.zdbjq.cn/Article/details/gjrikpayv.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.hesvh.cn/Article/details/ghqpemkda.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fehbvm.com/Article/details/gtywslpsp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fehbvm.com/Article/details/ggwwpbuyb.sHtML

[R47] sed 单行替换
来源：http://3g.zdbjq.cn/Article/details/gokqqvryc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.zdbjq.cn/Article/details/grqmcmldm.sHtML

[R48] awk 取指定列
来源：http://3g.zdbjq.cn/Article/details/gzjgtfvkl.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fehbvm.com/Article/details/gjpydsxfl.sHtML

[R49] awk 带条件
来源：http://www.m.share.zdbjq.cn/Article/details/gmppfmvdh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fehbvm.com/Article/details/gdxnsezyr.sHtML

[R50] awk 求和
来源：http://www.m.share.hesvh.cn/Article/details/gjoxlfyuk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gklmfckxn.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fehbvm.com/Article/details/grmqisikz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.hesvh.cn/Article/details/gmueshrye.sHtML

[R52] 统计行数
来源：http://3g.hesvh.cn/Article/details/gzmmxhlwv.sHtML

wc -l a.txt
来源：http://3g.zdbjq.cn/Article/details/gcjgnofgr.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.zdbjq.cn/Article/details/gqsxfjhtq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.hesvh.cn/Article/details/gfzrjxyom.sHtML

[R54] 比较两个文件
来源：http://www.blog.hesvh.cn/Article/details/gcydwpymy.sHtML

diff a.txt b.txt
来源：http://read.share.zdbjq.cn/Article/details/giihepvyd.sHtML

[R55] 压缩与解压
来源：http://mobile.fehbvm.com/Article/details/gbrdtgbhm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.zdbjq.cn/Article/details/grckizvyj.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gzkvypbak.sHtML

scp file user@host:/path/
来源：http://baike.hesvh.cn/Article/details/gxwawibip.sHtML

[R57] 远程执行命令
来源：http://read.share.hesvh.cn/Article/details/gbbuczsdq.sHtML

ssh user@host 'uptime'
来源：http://mobile.fehbvm.com/Article/details/gmamkeedx.sHtML

[R58] 下载文件
来源：http://mobile.fehbvm.com/Article/details/gszvbpntk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.hesvh.cn/Article/details/ggsukdodl.sHtML

[R59] 发 POST JSON
来源：http://wap.zdbjq.cn/Article/details/gdzkaithz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fehbvm.com/Article/details/gjmakawtv.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/gfkdkjrue.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fehbvm.com/Article/details/gulavlwuv.sHtML

[R61] 磁盘占用
来源：http://3g.fehbvm.com/Article/details/gbspqzzoz.sHtML

df -h;  du -sh *
来源：http://mobile.zdbjq.cn/Article/details/grksrxxfq.sHtML

[R62] 找最占空间的文件
来源：http://mobile.zdbjq.cn/Article/details/gpaycfgda.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.zdbjq.cn/Article/details/gnbprzimo.sHtML

[R63] 内存与进程
来源：http://www.share.hesvh.cn/Article/details/gmcjdxnyo.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fehbvm.com/Article/details/gljwokxsk.sHtML

[R64] 结束进程
来源：http://wap.zdbjq.cn/Article/details/gzmwuivcp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.zdbjq.cn/Article/details/gxphcakgt.sHtML

[R65] 查看端口占用
来源：http://www.m.share.zdbjq.cn/Article/details/gffzkxkyv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.zdbjq.cn/Article/details/gwlmrjwdd.sHtML

[R66] 定时任务
来源：http://blog.zdbjq.cn/Article/details/grhcpeehs.sHtML

crontab -e;  crontab -l
来源：http://wap.hesvh.cn/Article/details/ghgfagwjx.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fehbvm.com/Article/details/gfixkrjcy.sHtML

openssl rand -hex 16
来源：http://www.blog.zdbjq.cn/Article/details/gwxxbcjgc.sHtML

[R68] 计算文件校验值
来源：http://mobile.fehbvm.com/Article/details/ggcdepkrb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fehbvm.com/Article/details/gvffsevvp.sHtML

[R69] 生成随机密码
来源：http://www.share.fehbvm.com/Article/details/gepiqigfw.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fehbvm.com/Article/details/gaumnzbjc.sHtML

[R70] 时间戳与互转
来源：http://3g.zdbjq.cn/Article/details/gqflqqeql.sHtML

date +%s;  date -d @1700000000
来源：http://3g.zdbjq.cn/Article/details/gxsfsqceg.sHtML

[R71] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/gnihfgnlx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.hesvh.cn/Article/details/gmhxtoukt.sHtML

[R72] 等待端口就绪
来源：http://m.share.fehbvm.com/Article/details/gjwwwzemo.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/gernprwpn.sHtML

[R73] 分割大日志
来源：http://www.share.fehbvm.com/Article/details/glqzlqliw.sHtML

split -l 1000 big.log part_
来源：http://blog.zdbjq.cn/Article/details/gjarjqzlp.sHtML

[R74] 批量重命名
来源：http://baike.hesvh.cn/Article/details/gyoaiewnk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fehbvm.com/Article/details/gwyccmtkv.sHtML

[R75] 导出环境变量
来源：http://www.share.fehbvm.com/Article/details/gvohsnort.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fehbvm.com/Article/details/gbftahktb.sHtML

[R76] 使用临时文件
来源：http://blog.hesvh.cn/Article/details/gbclbneds.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/gnxasijug.sHtML

[R77] 读取用户输入
来源：http://www.m.share.hesvh.cn/Article/details/gxfqnjrnv.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fehbvm.com/Article/details/gbenionws.sHtML

[R78] 交互式菜单
来源：http://wap.fehbvm.com/Article/details/gfseszsta.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.hesvh.cn/Article/details/gwppahshr.sHtML

[R79] 解析命令行选项
来源：http://wap.zdbjq.cn/Article/details/gqnyiwqgz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.hesvh.cn/Article/details/gcernshvs.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fehbvm.com/Article/details/gezzovwpl.sHtML

time ./run.sh
来源：http://3g.zdbjq.cn/Article/details/gwqpsybti.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ghjbgtskr.sHtML

S. C / C++ 专题
来源：http://read.share.zdbjq.cn/Article/details/gqwhhurco.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gcvkvhgyt.sHtML

[S01] C：Hello World
来源：http://www.share.hesvh.cn/Article/details/gwhjgrogk.sHtML

#include <stdio.h>
来源：http://www.m.share.hesvh.cn/Article/details/ggvmvrvqw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fehbvm.com/Article/details/gzwrvcjyc.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.hesvh.cn/Article/details/gzewzbemy.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.hesvh.cn/Article/details/gaznclrsa.sHtML

[S03] C：读入整数
来源：http://blog.hesvh.cn/Article/details/gvwncrarv.sHtML

int x; scanf("%d", &x);
来源：http://read.share.zdbjq.cn/Article/details/guzjsowzd.sHtML

[S04] C：字符串复制
来源：http://blog.fehbvm.com/Article/details/gytasxqgh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.hesvh.cn/Article/details/gzpowjbmw.sHtML

[S05] C：字符串长度
来源：http://3g.zdbjq.cn/Article/details/galtedeef.sHtML

strlen(s)
来源：http://wap.hesvh.cn/Article/details/gagbluymu.sHtML

[S06] C：字符串比较
来源：http://wap.zdbjq.cn/Article/details/gdvowuurr.sHtML

strcmp(a, b) == 0
来源：http://www.share.zdbjq.cn/Article/details/gvlkwsgyr.sHtML

[S07] C：数组遍历求和
来源：http://mobile.hesvh.cn/Article/details/gyyqvmdvi.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.zdbjq.cn/Article/details/gbbykkkin.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.zdbjq.cn/Article/details/gpkdhahne.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.hesvh.cn/Article/details/groaqrfvb.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.zdbjq.cn/Article/details/gadmeiknp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.zdbjq.cn/Article/details/gkrnzqfxb.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fehbvm.com/Article/details/gmshdrkyd.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.zdbjq.cn/Article/details/grjspojgm.sHtML

[S11] C：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gwxlnpsct.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.zdbjq.cn/Article/details/gakjxdtbe.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.zdbjq.cn/Article/details/gyvjtegws.sHtML

fclose(f);
来源：http://3g.hesvh.cn/Article/details/gogsrclqh.sHtML

[S12] C：写文件
来源：http://3g.hesvh.cn/Article/details/grspnrbmb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/gnsbnpnsg.sHtML

[S13] C：宏定义
来源：http://3g.fehbvm.com/Article/details/gjgsntzri.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.zdbjq.cn/Article/details/gomvlusbi.sHtML

[S14] C：枚举
来源：http://wap.hesvh.cn/Article/details/gqyjqghjl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fehbvm.com/Article/details/gsgdmshfa.sHtML

[S15] C：类型转换
来源：http://wap.hesvh.cn/Article/details/gkbcaqhqy.sHtML

(double) a / b
来源：http://wap.zdbjq.cn/Article/details/glgpzochs.sHtML

[S16] C：位操作置位
来源：http://read.share.zdbjq.cn/Article/details/gavshdhvt.sHtML

x |= (1 << 3);
来源：http://baike.hesvh.cn/Article/details/gnukgqvff.sHtML

[S17] C：安全拼接字符串
来源：http://3g.hesvh.cn/Article/details/ghoarmtld.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.hesvh.cn/Article/details/gzulsxmsc.sHtML

[S18] C：命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/gvemqowuw.sHtML

int main(int argc, char **argv)
来源：http://blog.zdbjq.cn/Article/details/gvslauuxn.sHtML

[S19] C：快速排序
来源：http://wap.hesvh.cn/Article/details/gsrowtwlh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/gdxbidrfa.sHtML

[S20] C：二分查找
来源：http://blog.hesvh.cn/Article/details/gvtvxzwib.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gqngfvlwv.sHtML

[S21] C：字符类别判断
来源：http://www.blog.zdbjq.cn/Article/details/gchgbpkaf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fehbvm.com/Article/details/gpnctfqjx.sHtML

[S22] C：字符串转数字
来源：http://www.share.zdbjq.cn/Article/details/gyeeuohje.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fehbvm.com/Article/details/ggikslkgk.sHtML

[S23] C：随机数
来源：http://www.m.share.zdbjq.cn/Article/details/geeyqzfrx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.hesvh.cn/Article/details/gbeyoifpk.sHtML

[S24] C：获取本地时间
来源：http://m.share.zdbjq.cn/Article/details/gsezrmsya.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fehbvm.com/Article/details/guzcemrqq.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gptjnvrgq.sHtML

memcpy(dst, src, n);
来源：http://mobile.fehbvm.com/Article/details/gxhepchyr.sHtML

[S26] C：内存清零
来源：http://mobile.zdbjq.cn/Article/details/gtyfjsrri.sHtML

memset(a, 0, sizeof a);
来源：http://baike.hesvh.cn/Article/details/gpogirsfl.sHtML

[S27] C：定义常量
来源：http://3g.zdbjq.cn/Article/details/gdyighvef.sHtML

const double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gdjhfdkdj.sHtML

[S28] C：静态变量
来源：http://www.m.share.zdbjq.cn/Article/details/gyeyrlqbe.sHtML

static int counter = 0;
来源：http://www.m.share.fehbvm.com/Article/details/gzfkkbczn.sHtML

[S29] C：变参函数
来源：http://m.share.hesvh.cn/Article/details/gxpbyituw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.hesvh.cn/Article/details/gneidxoka.sHtML

[S30] C：头文件保护
来源：http://baike.zdbjq.cn/Article/details/gwvkaadyd.sHtML

#ifndef X_H
来源：http://www.share.zdbjq.cn/Article/details/gcjpmgsoy.sHtML

#define X_H
来源：http://blog.fehbvm.com/Article/details/gcxieredd.sHtML

#endif
来源：http://www.share.zdbjq.cn/Article/details/grnurfbik.sHtML

[S31] C++：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gurzsbygq.sHtML

#include <iostream>
来源：http://m.share.hesvh.cn/Article/details/gbvmpglip.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fehbvm.com/Article/details/gjlpdxeih.sHtML

[S32] C++：字符串
来源：http://blog.zdbjq.cn/Article/details/gyfsdioob.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fehbvm.com/Article/details/gtpehzvih.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fehbvm.com/Article/details/gaufqydqq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.hesvh.cn/Article/details/gfuouifvq.sHtML

[S34] C++：遍历 vector
来源：http://wap.hesvh.cn/Article/details/gncjubokh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.zdbjq.cn/Article/details/gnmrlsnqd.sHtML

[S35] C++：map
来源：http://www.m.share.zdbjq.cn/Article/details/gnjsrfcft.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/gfiqewrlr.sHtML

[S36] C++：unordered_map
来源：http://m.share.zdbjq.cn/Article/details/gbuwmeini.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/ghhlcqcyv.sHtML

[S37] C++：set
来源：http://www.share.hesvh.cn/Article/details/gpiitkwoa.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.hesvh.cn/Article/details/gvyenwnkt.sHtML

[S38] C++：排序
来源：http://www.share.fehbvm.com/Article/details/glaqfwqst.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fehbvm.com/Article/details/gewgeatqd.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.hesvh.cn/Article/details/gstujntnj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.zdbjq.cn/Article/details/gqvmoqocl.sHtML

[S40] C++：查找元素
来源：http://m.share.zdbjq.cn/Article/details/geolyswbr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fehbvm.com/Article/details/gzlpjftrd.sHtML

[S41] C++：类与构造函数
来源：http://3g.fehbvm.com/Article/details/geayqsrzt.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fehbvm.com/Article/details/gzinvcbxt.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fehbvm.com/Article/details/gbabgoqoj.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fehbvm.com/Article/details/gmjnbmggs.sHtML


<!-- 参考信息 -->