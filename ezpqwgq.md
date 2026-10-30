代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.hesvh.cn/Article/details/gjahmhypp.sHtML

[Q75] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/gpluvfjfk.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gxlcrragq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.hesvh.cn/Article/details/gcyvgtzfa.sHtML

[Q76] 按天统计
来源：http://mobile.fehbvm.com/Article/details/gbvjkqhbg.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fehbvm.com/Article/details/gqvjcisjd.sHtML

[Q77] 时间加减
来源：http://wap.hesvh.cn/Article/details/gdzsyeikq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fehbvm.com/Article/details/gcomjfwdb.sHtML

[Q78] 当前时间
来源：http://read.share.zdbjq.cn/Article/details/gapnqjkti.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.hesvh.cn/Article/details/gykestvyf.sHtML

[Q79] 字符串拼接
来源：http://wap.hesvh.cn/Article/details/gcobpdqwf.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.zdbjq.cn/Article/details/golhzhevp.sHtML

[Q80] 字符串截取
来源：http://mobile.zdbjq.cn/Article/details/gkudkyngt.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.hesvh.cn/Article/details/gkquvzolx.sHtML

[Q81] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/gtajqlezi.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.hesvh.cn/Article/details/gsfnyzftt.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fehbvm.com/Article/details/gzicnmszu.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gdyrsawrs.sHtML

[Q83] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gtyxhamcg.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gxchsxmdf.sHtML

[Q84] 去除首尾空格
来源：http://read.share.zdbjq.cn/Article/details/glfjyowzu.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gpvlhrvjg.sHtML

[Q85] 数值取整
来源：http://3g.fehbvm.com/Article/details/gtcgmvzeh.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fehbvm.com/Article/details/gnlugehgb.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.hesvh.cn/Article/details/gidsyucdt.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.hesvh.cn/Article/details/gidciqouj.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.hesvh.cn/Article/details/glrbgvydb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.hesvh.cn/Article/details/garubwcax.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.zdbjq.cn/Article/details/gpjripiqc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.zdbjq.cn/Article/details/gdgjbpmkz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.hesvh.cn/Article/details/gkladqrlp.sHtML

[Q89] 判断表是否存在
来源：http://3g.zdbjq.cn/Article/details/gnzbxlsxy.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fehbvm.com/Article/details/gdfefidro.sHtML

[Q90] 生成序号列
来源：http://baike.hesvh.cn/Article/details/gvqxjusaj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.zdbjq.cn/Article/details/gxlmewffa.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gmepuhdik.sHtML

R. Bash 专题
来源：http://www.blog.fehbvm.com/Article/details/gjlvreqmq.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gswayyuxb.sHtML

[R01] shebang 与严格模式
来源：http://m.share.zdbjq.cn/Article/details/gzzsygmkj.sHtML

#!/usr/bin/env bash
来源：http://mobile.zdbjq.cn/Article/details/gukctjswg.sHtML

set -euo pipefail
来源：http://mobile.zdbjq.cn/Article/details/gdeatbnzp.sHtML

[R02] 变量赋值与使用
来源：http://3g.zdbjq.cn/Article/details/gonqqdrae.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.hesvh.cn/Article/details/gnqqnicln.sHtML

[R03] 只读变量
来源：http://read.share.zdbjq.cn/Article/details/gfuxzghfd.sHtML

readonly PI=3.14
来源：http://www.blog.zdbjq.cn/Article/details/golticglz.sHtML

[R04] 位置参数
来源：http://m.share.fehbvm.com/Article/details/glaaaavxf.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.zdbjq.cn/Article/details/gxqandbjc.sHtML

[R05] 参数默认值
来源：http://read.share.hesvh.cn/Article/details/gelermxcf.sHtML

name="${1:-default}"
来源：http://www.share.zdbjq.cn/Article/details/goykeddxu.sHtML

[R06] 判断命令是否存在
来源：http://www.share.hesvh.cn/Article/details/gbgkpgoqk.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/gjccbubzn.sHtML

[R07] if 判断文件
来源：http://www.share.fehbvm.com/Article/details/gnfwoeaov.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fehbvm.com/Article/details/gxeugjnql.sHtML

[R08] 数值比较
来源：http://www.m.share.fehbvm.com/Article/details/grqpyqtsy.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.hesvh.cn/Article/details/gtooznomk.sHtML

[R09] 字符串比较
来源：http://read.share.fehbvm.com/Article/details/grrjvstrq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.zdbjq.cn/Article/details/gatevoxxp.sHtML

[R10] 正则匹配
来源：http://read.share.hesvh.cn/Article/details/gwjosixpw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.zdbjq.cn/Article/details/gxdzcgxwb.sHtML

[R11] case 多分支
来源：http://3g.zdbjq.cn/Article/details/gcvwiqfwn.sHtML

case "$1" in
来源：http://read.share.zdbjq.cn/Article/details/gnastlxgn.sHtML

start) echo "启动" ;;
来源：http://www.blog.hesvh.cn/Article/details/gqbwclwln.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gobeauupz.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.zdbjq.cn/Article/details/grvlnnlcq.sHtML

esac
来源：http://mobile.zdbjq.cn/Article/details/gobllfxjs.sHtML

[R12] for 遍历文件
来源：http://baike.fehbvm.com/Article/details/ggojmsdic.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.hesvh.cn/Article/details/gjajhvzna.sHtML

[R13] for 计数循环
来源：http://blog.hesvh.cn/Article/details/gluyjqvku.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/gmeuozpxe.sHtML

[R14] C 风格 for
来源：http://baike.hesvh.cn/Article/details/guslafvbf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/ghaymsnpa.sHtML

[R15] while 逐行读文件
来源：http://wap.hesvh.cn/Article/details/grdeqrfha.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.zdbjq.cn/Article/details/gglteupjq.sHtML

[R16] until 等待条件
来源：http://www.share.hesvh.cn/Article/details/gziizzeyz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.hesvh.cn/Article/details/gwcvfczsd.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.hesvh.cn/Article/details/gznshwmip.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.zdbjq.cn/Article/details/gcycmyrqp.sHtML

[R18] 遍历数组
来源：http://baike.fehbvm.com/Article/details/gananscup.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.zdbjq.cn/Article/details/gvfrrqlof.sHtML

[R19] 数组长度
来源：http://3g.fehbvm.com/Article/details/gecpvvldd.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.hesvh.cn/Article/details/gvbjfcqhz.sHtML

[R20] 关联数组（字典）
来源：http://www.share.hesvh.cn/Article/details/glszqdjbe.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.hesvh.cn/Article/details/gdtijiccn.sHtML

[R21] 字符串长度
来源：http://blog.fehbvm.com/Article/details/ggsjdqqrg.sHtML

echo "${#s}"
来源：http://blog.fehbvm.com/Article/details/gskaoeljw.sHtML

[R22] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/gpkfscwpw.sHtML

echo "${s:0:5}"
来源：http://wap.zdbjq.cn/Article/details/gfmuaemie.sHtML

[R23] 字符串替换
来源：http://www.m.share.hesvh.cn/Article/details/gblpmfrjs.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.zdbjq.cn/Article/details/gjznzmywz.sHtML

[R24] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gufpmaucp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fehbvm.com/Article/details/gsovugffr.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fehbvm.com/Article/details/gnkmquxau.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.hesvh.cn/Article/details/gjpbltccl.sHtML

[R26] 命令替换
来源：http://blog.hesvh.cn/Article/details/gjprpvznb.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fehbvm.com/Article/details/ghigucxmg.sHtML

[R27] 算术展开
来源：http://www.m.share.fehbvm.com/Article/details/geiqoahhy.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.zdbjq.cn/Article/details/gcgueqrup.sHtML

[R28] 浮点运算
来源：http://www.blog.hesvh.cn/Article/details/gzayaiusj.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.hesvh.cn/Article/details/gejwioqcg.sHtML

[R29] 定义函数
来源：http://wap.hesvh.cn/Article/details/gjqqwnnsk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.hesvh.cn/Article/details/gjhgnibgd.sHtML

[R30] 函数返回状态码
来源：http://read.share.fehbvm.com/Article/details/gctnbrfan.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fehbvm.com/Article/details/gfwhvuyzk.sHtML

[R31] 局部变量
来源：http://3g.fehbvm.com/Article/details/gvlfmidxe.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.hesvh.cn/Article/details/griehjsik.sHtML

[R32] 参数个数校验
来源：http://www.share.zdbjq.cn/Article/details/gopqalpyg.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/gvnetprto.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.hesvh.cn/Article/details/gpkzywylh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.zdbjq.cn/Article/details/gzdbekxvg.sHtML

[R34] 退出时清理
来源：http://baike.fehbvm.com/Article/details/gxxdctwxg.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gqzpyrgtn.sHtML

[R35] 后台执行并等待
来源：http://blog.hesvh.cn/Article/details/giefluzke.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.zdbjq.cn/Article/details/gumtpjyzq.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.hesvh.cn/Article/details/gzegqsoam.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.zdbjq.cn/Article/details/gcpmkujby.sHtML

[R37] 把输出赋给变量
来源：http://www.share.zdbjq.cn/Article/details/gapdrqvgt.sHtML

files=$(ls -1)
来源：http://wap.hesvh.cn/Article/details/gwdmatvnn.sHtML

[R38] 管道串联
来源：http://baike.zdbjq.cn/Article/details/gnlcjcqse.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fehbvm.com/Article/details/ggoluisgv.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fehbvm.com/Article/details/gexouuhtv.sHtML

cmd > out.log 2>&1
来源：http://m.share.hesvh.cn/Article/details/giwdjhrti.sHtML

[R40] 追加写日志
来源：http://blog.hesvh.cn/Article/details/gbcojnjga.sHtML

echo "log" >> out.log
来源：http://wap.hesvh.cn/Article/details/geiuczkif.sHtML

[R41] 丢弃输出
来源：http://mobile.hesvh.cn/Article/details/gnbmbdomz.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.hesvh.cn/Article/details/ghtwtzrbw.sHtML

[R42] 输入重定向
来源：http://www.m.share.zdbjq.cn/Article/details/ggkfixxne.sHtML

wc -l < a.txt
来源：http://read.share.zdbjq.cn/Article/details/gyofgwtjo.sHtML

[R43] 按名字查找文件
来源：http://read.share.zdbjq.cn/Article/details/glqbsndri.sHtML

find . -name "*.log" -type f
来源：http://wap.hesvh.cn/Article/details/gmddlwous.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fehbvm.com/Article/details/grnbjrtit.sHtML

find . -mtime -7 -type f
来源：http://3g.fehbvm.com/Article/details/gthxqpzze.sHtML

[R45] 批量删除
来源：http://www.m.share.zdbjq.cn/Article/details/gzrwgmtjg.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.zdbjq.cn/Article/details/gvgecglmc.sHtML

[R46] 递归替换文件内容
来源：http://blog.zdbjq.cn/Article/details/gmcfqjusl.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fehbvm.com/Article/details/gjyponuzs.sHtML

[R47] sed 单行替换
来源：http://3g.fehbvm.com/Article/details/gzjlvastj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.zdbjq.cn/Article/details/geinhbvzy.sHtML

[R48] awk 取指定列
来源：http://www.blog.zdbjq.cn/Article/details/gffkgvjtv.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.zdbjq.cn/Article/details/gadjbzupq.sHtML

[R49] awk 带条件
来源：http://3g.zdbjq.cn/Article/details/gsrqrqzsp.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fehbvm.com/Article/details/gjfwkytkn.sHtML

[R50] awk 求和
来源：http://www.share.fehbvm.com/Article/details/geqwpsyut.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fehbvm.com/Article/details/ggiluabwd.sHtML

[R51] 排序去重取前几
来源：http://wap.zdbjq.cn/Article/details/gdkxrhrwy.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.zdbjq.cn/Article/details/gjxbfopwi.sHtML

[R52] 统计行数
来源：http://baike.zdbjq.cn/Article/details/glzumcebo.sHtML

wc -l a.txt
来源：http://read.share.fehbvm.com/Article/details/gvkwbxqhv.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fehbvm.com/Article/details/gpiluwmte.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fehbvm.com/Article/details/gxmitdltd.sHtML

[R54] 比较两个文件
来源：http://mobile.hesvh.cn/Article/details/gjlempijr.sHtML

diff a.txt b.txt
来源：http://baike.hesvh.cn/Article/details/gcststkhw.sHtML

[R55] 压缩与解压
来源：http://mobile.zdbjq.cn/Article/details/geibmgjtz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.zdbjq.cn/Article/details/glqtejfhk.sHtML

[R56] 远程拷贝
来源：http://m.share.zdbjq.cn/Article/details/goojlfvhi.sHtML

scp file user@host:/path/
来源：http://baike.zdbjq.cn/Article/details/gmtfpstzh.sHtML

[R57] 远程执行命令
来源：http://blog.zdbjq.cn/Article/details/gmsecvpzu.sHtML

ssh user@host 'uptime'
来源：http://wap.hesvh.cn/Article/details/guyczmjtv.sHtML

[R58] 下载文件
来源：http://www.m.share.hesvh.cn/Article/details/gzksalvnb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.zdbjq.cn/Article/details/gtypkxdzj.sHtML

[R59] 发 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/gvwhhaole.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fehbvm.com/Article/details/gueupanaf.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/gnctvzeib.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.hesvh.cn/Article/details/gcxkpcrkm.sHtML

[R61] 磁盘占用
来源：http://wap.fehbvm.com/Article/details/gclsxzpvo.sHtML

df -h;  du -sh *
来源：http://m.share.fehbvm.com/Article/details/gbyllievq.sHtML

[R62] 找最占空间的文件
来源：http://blog.hesvh.cn/Article/details/gtenpdlyt.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fehbvm.com/Article/details/gpfrgrumn.sHtML

[R63] 内存与进程
来源：http://baike.fehbvm.com/Article/details/gfkplxdjw.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fehbvm.com/Article/details/gzsanyypb.sHtML

[R64] 结束进程
来源：http://read.share.fehbvm.com/Article/details/giyoteior.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.zdbjq.cn/Article/details/gbqoajrwv.sHtML

[R65] 查看端口占用
来源：http://wap.fehbvm.com/Article/details/gafdweqin.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.hesvh.cn/Article/details/gzjmwegyj.sHtML

[R66] 定时任务
来源：http://www.share.zdbjq.cn/Article/details/gxitwvhsc.sHtML

crontab -e;  crontab -l
来源：http://blog.hesvh.cn/Article/details/garzbsscb.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.hesvh.cn/Article/details/gypnduwxw.sHtML

openssl rand -hex 16
来源：http://mobile.hesvh.cn/Article/details/gwetcgcrv.sHtML

[R68] 计算文件校验值
来源：http://m.share.fehbvm.com/Article/details/gdeljrqzn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.hesvh.cn/Article/details/grixlredj.sHtML

[R69] 生成随机密码
来源：http://blog.fehbvm.com/Article/details/gnnresqim.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.hesvh.cn/Article/details/goykluiwh.sHtML

[R70] 时间戳与互转
来源：http://wap.fehbvm.com/Article/details/gtksipnqy.sHtML

date +%s;  date -d @1700000000
来源：http://wap.hesvh.cn/Article/details/gxrqsztjh.sHtML

[R71] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gcjhomyzt.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fehbvm.com/Article/details/gggkepztw.sHtML

[R72] 等待端口就绪
来源：http://read.share.fehbvm.com/Article/details/gpbpqjjfy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gljjrfguz.sHtML

[R73] 分割大日志
来源：http://m.share.zdbjq.cn/Article/details/gmuczbkpe.sHtML

split -l 1000 big.log part_
来源：http://www.share.fehbvm.com/Article/details/gendvznyn.sHtML

[R74] 批量重命名
来源：http://www.blog.hesvh.cn/Article/details/genvyffse.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.hesvh.cn/Article/details/gobsmmjgn.sHtML

[R75] 导出环境变量
来源：http://www.share.fehbvm.com/Article/details/gquxctudx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.hesvh.cn/Article/details/givuxezcd.sHtML

[R76] 使用临时文件
来源：http://www.blog.zdbjq.cn/Article/details/gtagnnhwn.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gwtqllsqc.sHtML

[R77] 读取用户输入
来源：http://m.share.hesvh.cn/Article/details/ghvxisvon.sHtML

read -rp "请输入: " ans
来源：http://www.share.fehbvm.com/Article/details/grxajwqjl.sHtML

[R78] 交互式菜单
来源：http://m.share.hesvh.cn/Article/details/gqsotlpzv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.zdbjq.cn/Article/details/givmoqgmi.sHtML

[R79] 解析命令行选项
来源：http://m.share.zdbjq.cn/Article/details/gsukvexee.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fehbvm.com/Article/details/gaovjndqz.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.hesvh.cn/Article/details/gncgufoqj.sHtML

time ./run.sh
来源：http://3g.hesvh.cn/Article/details/gawqseqiu.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/girttitss.sHtML

S. C / C++ 专题
来源：http://mobile.zdbjq.cn/Article/details/gisqvcinq.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gdabvwdxs.sHtML

[S01] C：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gcgiejkpq.sHtML

#include <stdio.h>
来源：http://blog.fehbvm.com/Article/details/ggghblomj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.hesvh.cn/Article/details/gzlqrdmar.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fehbvm.com/Article/details/gzupzjamd.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.zdbjq.cn/Article/details/gahkeaevm.sHtML

[S03] C：读入整数
来源：http://wap.hesvh.cn/Article/details/gpmoshmjk.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fehbvm.com/Article/details/geoqxxqkw.sHtML

[S04] C：字符串复制
来源：http://blog.zdbjq.cn/Article/details/gbufwxiwi.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.zdbjq.cn/Article/details/gkwdwqvbg.sHtML

[S05] C：字符串长度
来源：http://blog.hesvh.cn/Article/details/gorivzppc.sHtML

strlen(s)
来源：http://www.share.hesvh.cn/Article/details/gcfpptgvv.sHtML

[S06] C：字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gztizdykx.sHtML

strcmp(a, b) == 0
来源：http://3g.zdbjq.cn/Article/details/guhzjdziv.sHtML

[S07] C：数组遍历求和
来源：http://www.share.hesvh.cn/Article/details/glhydxgwq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fehbvm.com/Article/details/guxnbcrez.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fehbvm.com/Article/details/ggpbiuxwv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fehbvm.com/Article/details/gqtssbplu.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.hesvh.cn/Article/details/gyljlsmtm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fehbvm.com/Article/details/gvudcphsz.sHtML

[S10] C：指针与解引用
来源：http://blog.hesvh.cn/Article/details/glmqhliwm.sHtML

int *p = &a;  *p = 5;
来源：http://blog.hesvh.cn/Article/details/gimaktkqi.sHtML

[S11] C：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gcicggqeh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fehbvm.com/Article/details/gcmdxzwxe.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fehbvm.com/Article/details/gsmpeazcl.sHtML

fclose(f);
来源：http://baike.hesvh.cn/Article/details/gktclpuqt.sHtML

[S12] C：写文件
来源：http://read.share.zdbjq.cn/Article/details/gclpvpurj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/gquekrnfc.sHtML

[S13] C：宏定义
来源：http://read.share.fehbvm.com/Article/details/gqfhghust.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.zdbjq.cn/Article/details/gpezorzwb.sHtML

[S14] C：枚举
来源：http://wap.zdbjq.cn/Article/details/golnywszg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.zdbjq.cn/Article/details/gjzzfknce.sHtML

[S15] C：类型转换
来源：http://read.share.fehbvm.com/Article/details/gvkaltwex.sHtML

(double) a / b
来源：http://blog.zdbjq.cn/Article/details/goeysmznz.sHtML

[S16] C：位操作置位
来源：http://baike.fehbvm.com/Article/details/gapsrhfzy.sHtML

x |= (1 << 3);
来源：http://www.blog.zdbjq.cn/Article/details/gauzgxoty.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fehbvm.com/Article/details/glbspfajb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fehbvm.com/Article/details/gedvdxtqy.sHtML

[S18] C：命令行参数
来源：http://mobile.hesvh.cn/Article/details/gpjailvbl.sHtML

int main(int argc, char **argv)
来源：http://m.share.zdbjq.cn/Article/details/gmfbatmjs.sHtML

[S19] C：快速排序
来源：http://baike.zdbjq.cn/Article/details/grlsnhlxo.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/ghogwljht.sHtML

[S20] C：二分查找
来源：http://m.share.fehbvm.com/Article/details/gxycvujqx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gllbslegr.sHtML

[S21] C：字符类别判断
来源：http://www.share.zdbjq.cn/Article/details/ghmkvtjqa.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fehbvm.com/Article/details/guvuiiypf.sHtML

[S22] C：字符串转数字
来源：http://read.share.hesvh.cn/Article/details/gemfxjkrm.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.hesvh.cn/Article/details/gjzbptjvp.sHtML

[S23] C：随机数
来源：http://www.blog.zdbjq.cn/Article/details/gteydrbjd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fehbvm.com/Article/details/gjjlrpphe.sHtML

[S24] C：获取本地时间
来源：http://read.share.hesvh.cn/Article/details/goyryxnhi.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fehbvm.com/Article/details/gdjoduspk.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gdkmupnwo.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.hesvh.cn/Article/details/gqvuomcnd.sHtML

[S26] C：内存清零
来源：http://wap.zdbjq.cn/Article/details/gxdagjeae.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.zdbjq.cn/Article/details/gvuyrcdyq.sHtML

[S27] C：定义常量
来源：http://blog.fehbvm.com/Article/details/gkbuzneef.sHtML

const double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gtdlcjizw.sHtML

[S28] C：静态变量
来源：http://read.share.fehbvm.com/Article/details/gezuazfdf.sHtML

static int counter = 0;
来源：http://read.share.fehbvm.com/Article/details/govonhhsk.sHtML

[S29] C：变参函数
来源：http://www.share.fehbvm.com/Article/details/glpebijgi.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.zdbjq.cn/Article/details/gurrmdgpl.sHtML

[S30] C：头文件保护
来源：http://www.m.share.hesvh.cn/Article/details/gcwhuadnv.sHtML

#ifndef X_H
来源：http://m.share.fehbvm.com/Article/details/gsqakvaaj.sHtML

#define X_H
来源：http://3g.zdbjq.cn/Article/details/ghzrlnoct.sHtML

#endif
来源：http://baike.hesvh.cn/Article/details/gmhhtbllb.sHtML

[S31] C++：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gicwblglg.sHtML

#include <iostream>
来源：http://read.share.hesvh.cn/Article/details/ggsgoakri.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fehbvm.com/Article/details/gpetlxlcp.sHtML

[S32] C++：字符串
来源：http://wap.fehbvm.com/Article/details/golqtvxwa.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.zdbjq.cn/Article/details/ghvgbaidv.sHtML

[S33] C++：vector 增删
来源：http://m.share.hesvh.cn/Article/details/gmndewfxw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fehbvm.com/Article/details/girzetfvr.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fehbvm.com/Article/details/gqvipwvgt.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.hesvh.cn/Article/details/gdxgwbino.sHtML

[S35] C++：map
来源：http://www.m.share.fehbvm.com/Article/details/gkfdddsnm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/goehskmgu.sHtML

[S36] C++：unordered_map
来源：http://mobile.hesvh.cn/Article/details/gcfselayy.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/gkklwwypo.sHtML

[S37] C++：set
来源：http://wap.fehbvm.com/Article/details/gbyezhkhr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fehbvm.com/Article/details/gwpjlhaai.sHtML

[S38] C++：排序
来源：http://www.share.fehbvm.com/Article/details/glbfmxdby.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.zdbjq.cn/Article/details/gijdofbtr.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.zdbjq.cn/Article/details/gkzqtjbxs.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.hesvh.cn/Article/details/ggqhilfxa.sHtML

[S40] C++：查找元素
来源：http://www.share.zdbjq.cn/Article/details/gpybzldav.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fehbvm.com/Article/details/gzrwhsyyb.sHtML

[S41] C++：类与构造函数
来源：http://wap.zdbjq.cn/Article/details/guehkspdt.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fehbvm.com/Article/details/ggjcnbtad.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fehbvm.com/Article/details/gngkseagf.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fehbvm.com/Article/details/gwmofvnms.sHtML

[S43] C++：智能指针
来源：http://mobile.fehbvm.com/Article/details/guyxyrofg.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fehbvm.com/Article/details/gwelbnjca.sHtML

[S44] C++：引用传参
来源：http://www.share.zdbjq.cn/Article/details/gwkmfoxar.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.hesvh.cn/Article/details/gtrzyvfya.sHtML


<!-- 参考信息 -->