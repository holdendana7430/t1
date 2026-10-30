代发 wailian999

ANALYZE TABLE users;
来源：http://3g.zdbjq.cn/Article/details/gypuuoajg.sHtML

[Q71] 查看建表语句
来源：http://mobile.zdbjq.cn/Article/details/geaozuovh.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.zdbjq.cn/Article/details/gzqlnexgo.sHtML

[Q72] 查看索引
来源：http://3g.hesvh.cn/Article/details/gmwdjbkfc.sHtML

SHOW INDEX FROM users;
来源：http://3g.zdbjq.cn/Article/details/gwhtyaawg.sHtML

[Q73] 查看表状态
来源：http://read.share.hesvh.cn/Article/details/glawvfknf.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fehbvm.com/Article/details/gmedaecdg.sHtML

[Q74] 强制使用索引
来源：http://m.share.hesvh.cn/Article/details/gnyougdvq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.hesvh.cn/Article/details/gosxasaos.sHtML

[Q75] 日期格式化
来源：http://3g.fehbvm.com/Article/details/gudugmqft.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gtsttyggi.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fehbvm.com/Article/details/gukbpqulg.sHtML

[Q76] 按天统计
来源：http://3g.zdbjq.cn/Article/details/gkckjycyf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fehbvm.com/Article/details/gohosjcxv.sHtML

[Q77] 时间加减
来源：http://baike.hesvh.cn/Article/details/ghfvgtsxf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fehbvm.com/Article/details/gloysngqa.sHtML

[Q78] 当前时间
来源：http://baike.zdbjq.cn/Article/details/gmlcaqjgv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.zdbjq.cn/Article/details/gkwjbyyvw.sHtML

[Q79] 字符串拼接
来源：http://read.share.hesvh.cn/Article/details/glrejtpna.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fehbvm.com/Article/details/gpuinqgyc.sHtML

[Q80] 字符串截取
来源：http://www.share.zdbjq.cn/Article/details/gomjpuihs.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gmhhvhfya.sHtML

[Q81] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/ggyfyhwhk.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/geokvqhsn.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.zdbjq.cn/Article/details/gadgvxerd.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gzhjlobcj.sHtML

[Q83] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gmqtogugi.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/grlzflzyv.sHtML

[Q84] 去除首尾空格
来源：http://baike.hesvh.cn/Article/details/goigpvqgd.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gsbsogcty.sHtML

[Q85] 数值取整
来源：http://m.share.zdbjq.cn/Article/details/gaxogxwvz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.zdbjq.cn/Article/details/gxyepscpd.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.zdbjq.cn/Article/details/gwfbqhhdi.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.hesvh.cn/Article/details/gyzlnkerr.sHtML

[Q87] JSON 字段做条件
来源：http://3g.zdbjq.cn/Article/details/gynlnwhbb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.zdbjq.cn/Article/details/gbtkkzlor.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.zdbjq.cn/Article/details/gnrrkevvd.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fehbvm.com/Article/details/gmwzcyqxr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fehbvm.com/Article/details/guvrpsbzt.sHtML

[Q89] 判断表是否存在
来源：http://baike.hesvh.cn/Article/details/ghmbodzed.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.zdbjq.cn/Article/details/ghibjgwsj.sHtML

[Q90] 生成序号列
来源：http://m.share.fehbvm.com/Article/details/gvscrjlvj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fehbvm.com/Article/details/gnfconfzr.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gaaicxnvf.sHtML

R. Bash 专题
来源：http://www.blog.fehbvm.com/Article/details/gmztzgzhb.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gznocmytu.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fehbvm.com/Article/details/gtzjqncmq.sHtML

#!/usr/bin/env bash
来源：http://m.share.hesvh.cn/Article/details/gjovcnjyt.sHtML

set -euo pipefail
来源：http://read.share.hesvh.cn/Article/details/girchmusi.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fehbvm.com/Article/details/gubgunubs.sHtML

name="Tom"; echo "$name"
来源：http://www.share.zdbjq.cn/Article/details/giylodnxe.sHtML

[R03] 只读变量
来源：http://read.share.zdbjq.cn/Article/details/gewbjyror.sHtML

readonly PI=3.14
来源：http://blog.zdbjq.cn/Article/details/gmokebnnn.sHtML

[R04] 位置参数
来源：http://3g.zdbjq.cn/Article/details/gscsabolm.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fehbvm.com/Article/details/gsjknbfoh.sHtML

[R05] 参数默认值
来源：http://www.m.share.zdbjq.cn/Article/details/giizkxbzv.sHtML

name="${1:-default}"
来源：http://wap.fehbvm.com/Article/details/gdwuynjox.sHtML

[R06] 判断命令是否存在
来源：http://baike.hesvh.cn/Article/details/gdkmwahah.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/gffotyxwg.sHtML

[R07] if 判断文件
来源：http://read.share.hesvh.cn/Article/details/gndfnkeyg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.hesvh.cn/Article/details/grzzwqzsn.sHtML

[R08] 数值比较
来源：http://read.share.fehbvm.com/Article/details/grcwwkuxy.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.zdbjq.cn/Article/details/gogaiijnb.sHtML

[R09] 字符串比较
来源：http://3g.zdbjq.cn/Article/details/glfeqgsfc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.hesvh.cn/Article/details/gleuwdunm.sHtML

[R10] 正则匹配
来源：http://wap.fehbvm.com/Article/details/guoesfsok.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gtpmepmnm.sHtML

[R11] case 多分支
来源：http://www.m.share.zdbjq.cn/Article/details/gbxhlmxyq.sHtML

case "$1" in
来源：http://read.share.zdbjq.cn/Article/details/gricfgxpq.sHtML

start) echo "启动" ;;
来源：http://wap.hesvh.cn/Article/details/gckuqtprm.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gjtvlyhlx.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gndebdkta.sHtML

esac
来源：http://blog.zdbjq.cn/Article/details/gaatfqwfq.sHtML

[R12] for 遍历文件
来源：http://read.share.hesvh.cn/Article/details/gyhliypuc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.zdbjq.cn/Article/details/gtshulmmc.sHtML

[R13] for 计数循环
来源：http://mobile.zdbjq.cn/Article/details/gophqbnbf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/gwgrktsse.sHtML

[R14] C 风格 for
来源：http://m.share.fehbvm.com/Article/details/guqavupgb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/goxfbdgyq.sHtML

[R15] while 逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gpnvvbxdd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.zdbjq.cn/Article/details/gasoibfln.sHtML

[R16] until 等待条件
来源：http://read.share.hesvh.cn/Article/details/gwdmgxkbn.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/gnhtuirpb.sHtML

[R17] 数组定义与取值
来源：http://read.share.hesvh.cn/Article/details/ghkjnsuce.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.zdbjq.cn/Article/details/gluzxjdll.sHtML

[R18] 遍历数组
来源：http://read.share.fehbvm.com/Article/details/gniegmmyv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.zdbjq.cn/Article/details/gwxafdxqu.sHtML

[R19] 数组长度
来源：http://baike.fehbvm.com/Article/details/ggrhorwnz.sHtML

echo "${#arr[@]}"
来源：http://baike.hesvh.cn/Article/details/glqoxnfmg.sHtML

[R20] 关联数组（字典）
来源：http://3g.hesvh.cn/Article/details/gryrtdvyo.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gdwxktrsh.sHtML

[R21] 字符串长度
来源：http://www.blog.fehbvm.com/Article/details/gjrllclrt.sHtML

echo "${#s}"
来源：http://mobile.zdbjq.cn/Article/details/ganrfsizr.sHtML

[R22] 截取子串
来源：http://wap.hesvh.cn/Article/details/gwwjjplct.sHtML

echo "${s:0:5}"
来源：http://mobile.zdbjq.cn/Article/details/gsqqnunbi.sHtML

[R23] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/gbsyhhunc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.hesvh.cn/Article/details/gmmoheclm.sHtML

[R24] 大小写转换
来源：http://blog.fehbvm.com/Article/details/ggpzpacgo.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.hesvh.cn/Article/details/gfpfppxlk.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.hesvh.cn/Article/details/ggyyjptgf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.zdbjq.cn/Article/details/gqbnpmbks.sHtML

[R26] 命令替换
来源：http://3g.zdbjq.cn/Article/details/gmqflpyme.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.zdbjq.cn/Article/details/gbcxvevwy.sHtML

[R27] 算术展开
来源：http://www.m.share.hesvh.cn/Article/details/gshwbiftb.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.zdbjq.cn/Article/details/gdgauwgii.sHtML

[R28] 浮点运算
来源：http://baike.fehbvm.com/Article/details/ghmgnykmb.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fehbvm.com/Article/details/gijluzmfg.sHtML

[R29] 定义函数
来源：http://m.share.fehbvm.com/Article/details/gkbnqlgti.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fehbvm.com/Article/details/genuouhuk.sHtML

[R30] 函数返回状态码
来源：http://blog.fehbvm.com/Article/details/glkninqty.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.hesvh.cn/Article/details/gveailtqb.sHtML

[R31] 局部变量
来源：http://3g.fehbvm.com/Article/details/gzxauoejx.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.hesvh.cn/Article/details/gdjntaugp.sHtML

[R32] 参数个数校验
来源：http://baike.fehbvm.com/Article/details/gqgozyjdu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.hesvh.cn/Article/details/gpudnwfpq.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.zdbjq.cn/Article/details/gochnwwcr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.hesvh.cn/Article/details/gvelhehgn.sHtML

[R34] 退出时清理
来源：http://wap.fehbvm.com/Article/details/gopnebnlq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gdqkrnnwp.sHtML

[R35] 后台执行并等待
来源：http://m.share.hesvh.cn/Article/details/gqpnsmptj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.hesvh.cn/Article/details/gortsvycs.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fehbvm.com/Article/details/gszknjtdc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.zdbjq.cn/Article/details/geyuofulo.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fehbvm.com/Article/details/guerpsuqx.sHtML

files=$(ls -1)
来源：http://3g.fehbvm.com/Article/details/gvtxcidoq.sHtML

[R38] 管道串联
来源：http://www.blog.hesvh.cn/Article/details/gzwzjdpgc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fehbvm.com/Article/details/gbmruvmkh.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.zdbjq.cn/Article/details/gjamhntzy.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gyyertldm.sHtML

[R40] 追加写日志
来源：http://blog.fehbvm.com/Article/details/gfqdxpuhe.sHtML

echo "log" >> out.log
来源：http://baike.zdbjq.cn/Article/details/gquqcbmse.sHtML

[R41] 丢弃输出
来源：http://baike.hesvh.cn/Article/details/gfgsiuhbs.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fehbvm.com/Article/details/ghhtqrjvt.sHtML

[R42] 输入重定向
来源：http://blog.fehbvm.com/Article/details/gwznphvcv.sHtML

wc -l < a.txt
来源：http://mobile.zdbjq.cn/Article/details/garhvgixe.sHtML

[R43] 按名字查找文件
来源：http://wap.hesvh.cn/Article/details/ghljlaczi.sHtML

find . -name "*.log" -type f
来源：http://blog.fehbvm.com/Article/details/gaazaogvt.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.hesvh.cn/Article/details/gjtakqjst.sHtML

find . -mtime -7 -type f
来源：http://read.share.fehbvm.com/Article/details/ghgaltzpk.sHtML

[R45] 批量删除
来源：http://read.share.hesvh.cn/Article/details/gvvzsqeve.sHtML

find . -name "*.tmp" -delete
来源：http://3g.hesvh.cn/Article/details/gfwrzlrjv.sHtML

[R46] 递归替换文件内容
来源：http://wap.hesvh.cn/Article/details/gtpznngef.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.hesvh.cn/Article/details/giglmkphp.sHtML

[R47] sed 单行替换
来源：http://www.m.share.zdbjq.cn/Article/details/gzuvrcuji.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fehbvm.com/Article/details/gjsjawnnm.sHtML

[R48] awk 取指定列
来源：http://read.share.zdbjq.cn/Article/details/gihneuqhw.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gyhbrepdk.sHtML

[R49] awk 带条件
来源：http://baike.hesvh.cn/Article/details/gtmnmenrr.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.zdbjq.cn/Article/details/gdazsxona.sHtML

[R50] awk 求和
来源：http://www.m.share.hesvh.cn/Article/details/gznonoexn.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.hesvh.cn/Article/details/gjmexmqsw.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.zdbjq.cn/Article/details/glipgmrtc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.hesvh.cn/Article/details/ggvqabdwt.sHtML

[R52] 统计行数
来源：http://blog.fehbvm.com/Article/details/gxrzquykb.sHtML

wc -l a.txt
来源：http://m.share.hesvh.cn/Article/details/gwqgclcjt.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.hesvh.cn/Article/details/gafjyntji.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.hesvh.cn/Article/details/gtfqrqath.sHtML

[R54] 比较两个文件
来源：http://www.share.zdbjq.cn/Article/details/gjychmwqx.sHtML

diff a.txt b.txt
来源：http://www.blog.fehbvm.com/Article/details/gaufhgits.sHtML

[R55] 压缩与解压
来源：http://read.share.hesvh.cn/Article/details/gutvrfpbm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.zdbjq.cn/Article/details/gvohaapmy.sHtML

[R56] 远程拷贝
来源：http://www.share.fehbvm.com/Article/details/gnnokjwpu.sHtML

scp file user@host:/path/
来源：http://blog.zdbjq.cn/Article/details/gbjollaku.sHtML

[R57] 远程执行命令
来源：http://wap.fehbvm.com/Article/details/gpyecefis.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fehbvm.com/Article/details/gfyooznjk.sHtML

[R58] 下载文件
来源：http://baike.fehbvm.com/Article/details/gpspcgxig.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fehbvm.com/Article/details/gugkbmwjx.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fehbvm.com/Article/details/gsfkuipok.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.hesvh.cn/Article/details/guhilbjhl.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/gvixqtnir.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.zdbjq.cn/Article/details/gcxdrbmtb.sHtML

[R61] 磁盘占用
来源：http://www.m.share.zdbjq.cn/Article/details/gwvioyqxx.sHtML

df -h;  du -sh *
来源：http://wap.zdbjq.cn/Article/details/gsnrieuvz.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fehbvm.com/Article/details/gpedjqcfv.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.zdbjq.cn/Article/details/gliykrmsh.sHtML

[R63] 内存与进程
来源：http://3g.zdbjq.cn/Article/details/grfcnopkm.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.hesvh.cn/Article/details/gsbkqwjgq.sHtML

[R64] 结束进程
来源：http://blog.fehbvm.com/Article/details/gshmbpwkv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.zdbjq.cn/Article/details/gjdkxzkzl.sHtML

[R65] 查看端口占用
来源：http://www.share.hesvh.cn/Article/details/gnryrfomc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.hesvh.cn/Article/details/gqveyefsn.sHtML

[R66] 定时任务
来源：http://read.share.hesvh.cn/Article/details/gfoaommfb.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.hesvh.cn/Article/details/gfxzmphfm.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fehbvm.com/Article/details/grweqpowf.sHtML

openssl rand -hex 16
来源：http://blog.zdbjq.cn/Article/details/ghfftmgao.sHtML

[R68] 计算文件校验值
来源：http://www.share.hesvh.cn/Article/details/gdhlpcbnu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.hesvh.cn/Article/details/gtrilwdpx.sHtML

[R69] 生成随机密码
来源：http://wap.zdbjq.cn/Article/details/gpoyomjop.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fehbvm.com/Article/details/ghphtbvun.sHtML

[R70] 时间戳与互转
来源：http://m.share.hesvh.cn/Article/details/gavhiqqui.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.hesvh.cn/Article/details/gsaiesabl.sHtML

[R71] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/givmuzgyc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.zdbjq.cn/Article/details/gnfapwcik.sHtML

[R72] 等待端口就绪
来源：http://3g.zdbjq.cn/Article/details/gfcpobniz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gpqkzqbkj.sHtML

[R73] 分割大日志
来源：http://mobile.hesvh.cn/Article/details/gnlfgsppj.sHtML

split -l 1000 big.log part_
来源：http://blog.zdbjq.cn/Article/details/gcjrpmbzs.sHtML

[R74] 批量重命名
来源：http://www.m.share.fehbvm.com/Article/details/gimyanrdl.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fehbvm.com/Article/details/gkahohuaf.sHtML

[R75] 导出环境变量
来源：http://www.blog.fehbvm.com/Article/details/gsvziinqw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fehbvm.com/Article/details/giovutlda.sHtML

[R76] 使用临时文件
来源：http://mobile.zdbjq.cn/Article/details/gwfaoxhre.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gejicdgnd.sHtML

[R77] 读取用户输入
来源：http://baike.zdbjq.cn/Article/details/glwlivsma.sHtML

read -rp "请输入: " ans
来源：http://wap.zdbjq.cn/Article/details/glzbfqzmf.sHtML

[R78] 交互式菜单
来源：http://wap.hesvh.cn/Article/details/gnhyjnbcc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.hesvh.cn/Article/details/gahudsddw.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fehbvm.com/Article/details/gabarotxf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.zdbjq.cn/Article/details/gumffprhn.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fehbvm.com/Article/details/gjfilpncq.sHtML

time ./run.sh
来源：http://blog.hesvh.cn/Article/details/gbrtsecvl.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gqtvlskbu.sHtML

S. C / C++ 专题
来源：http://read.share.zdbjq.cn/Article/details/gprdtmtzi.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gvthmdqjo.sHtML

[S01] C：Hello World
来源：http://blog.hesvh.cn/Article/details/gdnidgyso.sHtML

#include <stdio.h>
来源：http://blog.fehbvm.com/Article/details/groxvzziu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.hesvh.cn/Article/details/gvyvnckcc.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fehbvm.com/Article/details/gkodneiss.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.hesvh.cn/Article/details/gegidwgfi.sHtML

[S03] C：读入整数
来源：http://www.m.share.zdbjq.cn/Article/details/gykqxuniv.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fehbvm.com/Article/details/gricaaujp.sHtML

[S04] C：字符串复制
来源：http://3g.zdbjq.cn/Article/details/gtaremkbj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fehbvm.com/Article/details/gfilrlyzr.sHtML

[S05] C：字符串长度
来源：http://3g.fehbvm.com/Article/details/gicbpsjib.sHtML

strlen(s)
来源：http://www.m.share.fehbvm.com/Article/details/glqwirqma.sHtML

[S06] C：字符串比较
来源：http://3g.hesvh.cn/Article/details/gthdegous.sHtML

strcmp(a, b) == 0
来源：http://m.share.zdbjq.cn/Article/details/goqtdxjhb.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fehbvm.com/Article/details/gvmwpzojq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.zdbjq.cn/Article/details/guyxiccip.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.hesvh.cn/Article/details/gakuzlidr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.zdbjq.cn/Article/details/gihmbbwmc.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fehbvm.com/Article/details/gytppjtoz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.zdbjq.cn/Article/details/gqgdboayc.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.zdbjq.cn/Article/details/gqmynlafg.sHtML

int *p = &a;  *p = 5;
来源：http://baike.hesvh.cn/Article/details/gnumczhnx.sHtML

[S11] C：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gcmxalqzg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.hesvh.cn/Article/details/gdbmiqaxu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fehbvm.com/Article/details/gzrhmawct.sHtML

fclose(f);
来源：http://3g.hesvh.cn/Article/details/gmofqkmih.sHtML

[S12] C：写文件
来源：http://www.share.hesvh.cn/Article/details/gihrfliuu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/gipxbymcc.sHtML

[S13] C：宏定义
来源：http://www.m.share.fehbvm.com/Article/details/gajdyzoqg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fehbvm.com/Article/details/gcuudfafi.sHtML

[S14] C：枚举
来源：http://baike.zdbjq.cn/Article/details/gainidwma.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.zdbjq.cn/Article/details/gulroqcpr.sHtML

[S15] C：类型转换
来源：http://m.share.zdbjq.cn/Article/details/gjxsyigay.sHtML

(double) a / b
来源：http://blog.zdbjq.cn/Article/details/gfbphzkpd.sHtML

[S16] C：位操作置位
来源：http://3g.zdbjq.cn/Article/details/gzdeavtot.sHtML

x |= (1 << 3);
来源：http://wap.fehbvm.com/Article/details/gbxbcyvxl.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/ggsefjwqc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.zdbjq.cn/Article/details/geehdqdgi.sHtML

[S18] C：命令行参数
来源：http://wap.zdbjq.cn/Article/details/gcjztczxn.sHtML

int main(int argc, char **argv)
来源：http://www.blog.hesvh.cn/Article/details/gpeukusoy.sHtML

[S19] C：快速排序
来源：http://baike.hesvh.cn/Article/details/gadzecccs.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/grclgzbzf.sHtML

[S20] C：二分查找
来源：http://wap.zdbjq.cn/Article/details/gljtqcezd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/gkpnrfhjb.sHtML

[S21] C：字符类别判断
来源：http://www.share.zdbjq.cn/Article/details/goizaufsl.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.zdbjq.cn/Article/details/gupwczcig.sHtML

[S22] C：字符串转数字
来源：http://www.blog.hesvh.cn/Article/details/gdnekunqr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fehbvm.com/Article/details/gljxqmxxp.sHtML

[S23] C：随机数
来源：http://baike.hesvh.cn/Article/details/gjtfuesyq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.hesvh.cn/Article/details/gedxgcldf.sHtML

[S24] C：获取本地时间
来源：http://3g.zdbjq.cn/Article/details/ggxrzkibm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fehbvm.com/Article/details/gwarjmhvy.sHtML

[S25] C：内存拷贝
来源：http://wap.fehbvm.com/Article/details/gyxzmifiu.sHtML

memcpy(dst, src, n);
来源：http://wap.hesvh.cn/Article/details/gasoqbzyo.sHtML

[S26] C：内存清零
来源：http://mobile.hesvh.cn/Article/details/gbwqmywcu.sHtML

memset(a, 0, sizeof a);
来源：http://wap.hesvh.cn/Article/details/grayrjdin.sHtML

[S27] C：定义常量
来源：http://baike.fehbvm.com/Article/details/gsfvecklp.sHtML

const double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gyxceykdp.sHtML

[S28] C：静态变量
来源：http://www.m.share.fehbvm.com/Article/details/gkdxkqltb.sHtML

static int counter = 0;
来源：http://wap.zdbjq.cn/Article/details/gxiorjuld.sHtML

[S29] C：变参函数
来源：http://mobile.zdbjq.cn/Article/details/gijkdlpif.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.zdbjq.cn/Article/details/gkrjjocez.sHtML

[S30] C：头文件保护
来源：http://baike.zdbjq.cn/Article/details/gzhvmgwej.sHtML

#ifndef X_H
来源：http://www.blog.zdbjq.cn/Article/details/gbkdnaggx.sHtML

#define X_H
来源：http://m.share.zdbjq.cn/Article/details/gcciyiorl.sHtML

#endif
来源：http://www.blog.fehbvm.com/Article/details/greuxtksu.sHtML

[S31] C++：Hello World
来源：http://baike.fehbvm.com/Article/details/gorucjiqj.sHtML

#include <iostream>
来源：http://baike.fehbvm.com/Article/details/gzmxthmfw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.hesvh.cn/Article/details/goknfiidb.sHtML

[S32] C++：字符串
来源：http://baike.zdbjq.cn/Article/details/gvvklleag.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.hesvh.cn/Article/details/gfepjasrz.sHtML

[S33] C++：vector 增删
来源：http://wap.zdbjq.cn/Article/details/gizjwvfgn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fehbvm.com/Article/details/genvlziks.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fehbvm.com/Article/details/gqfsiipcx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.zdbjq.cn/Article/details/gehovxzds.sHtML

[S35] C++：map
来源：http://blog.fehbvm.com/Article/details/getbxyrrb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/gofgomdja.sHtML

[S36] C++：unordered_map
来源：http://blog.hesvh.cn/Article/details/gethaalbq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gocsaxcql.sHtML

[S37] C++：set
来源：http://mobile.zdbjq.cn/Article/details/guzbqqfem.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fehbvm.com/Article/details/gsutrptxb.sHtML

[S38] C++：排序
来源：http://3g.zdbjq.cn/Article/details/gxydbqezz.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gmckoofln.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fehbvm.com/Article/details/gmgmzvnuw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fehbvm.com/Article/details/gpfvgjgtl.sHtML

[S40] C++：查找元素
来源：http://mobile.zdbjq.cn/Article/details/gddpigeae.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.hesvh.cn/Article/details/girsryzqo.sHtML


<!-- 参考信息 -->