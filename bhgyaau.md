代发 wailian999

[Q78] 当前时间
来源：http://baike.hesvh.cn/Article/details/gbeksoiyy.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.hesvh.cn/Article/details/gvgbmibov.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.hesvh.cn/Article/details/gtgxpucfx.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.hesvh.cn/Article/details/gzlpneipt.sHtML

[Q80] 字符串截取
来源：http://blog.hesvh.cn/Article/details/gruqiwuvs.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/ghgleyeoa.sHtML

[Q81] 字符串替换
来源：http://blog.fehbvm.com/Article/details/gsicfqlak.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.hesvh.cn/Article/details/gadesawqo.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fehbvm.com/Article/details/gzvjclpdg.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gbtuzobkb.sHtML

[Q83] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gkyyqxayi.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/ggrwfkild.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fehbvm.com/Article/details/gcyyfpbht.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gzxjzvhux.sHtML

[Q85] 数值取整
来源：http://m.share.hesvh.cn/Article/details/goahbeiyx.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.hesvh.cn/Article/details/gcwbobgyt.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.hesvh.cn/Article/details/gshcxvjdo.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.zdbjq.cn/Article/details/gffxlzsqw.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fehbvm.com/Article/details/grtpvuuqb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.hesvh.cn/Article/details/ghxziqioq.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.zdbjq.cn/Article/details/gfwlksyjh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.zdbjq.cn/Article/details/gvinqasba.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fehbvm.com/Article/details/gshkhemnm.sHtML

[Q89] 判断表是否存在
来源：http://blog.hesvh.cn/Article/details/gzfcldcgb.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.hesvh.cn/Article/details/gvwbmunhs.sHtML

[Q90] 生成序号列
来源：http://read.share.fehbvm.com/Article/details/goijrkcvd.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fehbvm.com/Article/details/gvjouenga.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gpxjfwtnw.sHtML

R. Bash 专题
来源：http://www.blog.zdbjq.cn/Article/details/grjepoopa.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ghrajdolk.sHtML

[R01] shebang 与严格模式
来源：http://blog.hesvh.cn/Article/details/glygdwwng.sHtML

#!/usr/bin/env bash
来源：http://m.share.zdbjq.cn/Article/details/gcekpotpc.sHtML

set -euo pipefail
来源：http://read.share.zdbjq.cn/Article/details/gnccxvgmw.sHtML

[R02] 变量赋值与使用
来源：http://baike.fehbvm.com/Article/details/gplxllrwo.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.hesvh.cn/Article/details/gcrykaqqs.sHtML

[R03] 只读变量
来源：http://read.share.zdbjq.cn/Article/details/gvuqkwucw.sHtML

readonly PI=3.14
来源：http://baike.zdbjq.cn/Article/details/giefzganc.sHtML

[R04] 位置参数
来源：http://www.blog.hesvh.cn/Article/details/ganppavoo.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.hesvh.cn/Article/details/gjjvatlek.sHtML

[R05] 参数默认值
来源：http://baike.zdbjq.cn/Article/details/ghzbnvyyh.sHtML

name="${1:-default}"
来源：http://wap.hesvh.cn/Article/details/gsabaqhjg.sHtML

[R06] 判断命令是否存在
来源：http://wap.fehbvm.com/Article/details/gvfnbqkae.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/gxrruzfcm.sHtML

[R07] if 判断文件
来源：http://mobile.zdbjq.cn/Article/details/ggpqcktyl.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fehbvm.com/Article/details/gaghtxvob.sHtML

[R08] 数值比较
来源：http://baike.hesvh.cn/Article/details/gpdndeqwt.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.zdbjq.cn/Article/details/gnzewlkml.sHtML

[R09] 字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gsjxmsrwy.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.zdbjq.cn/Article/details/gvnkttvpn.sHtML

[R10] 正则匹配
来源：http://baike.zdbjq.cn/Article/details/gaemenwat.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.zdbjq.cn/Article/details/ghwragshl.sHtML

[R11] case 多分支
来源：http://mobile.hesvh.cn/Article/details/goffwjnul.sHtML

case "$1" in
来源：http://blog.zdbjq.cn/Article/details/gtrkkdmkt.sHtML

start) echo "启动" ;;
来源：http://m.share.hesvh.cn/Article/details/gaqudvyaf.sHtML

stop)  echo "停止" ;;
来源：http://wap.zdbjq.cn/Article/details/ghdwmfwrs.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.zdbjq.cn/Article/details/gcyxvxvxs.sHtML

esac
来源：http://3g.fehbvm.com/Article/details/gqtfzjesl.sHtML

[R12] for 遍历文件
来源：http://read.share.zdbjq.cn/Article/details/gkvzmmobh.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.zdbjq.cn/Article/details/gksreqvqo.sHtML

[R13] for 计数循环
来源：http://www.m.share.zdbjq.cn/Article/details/gokpblhau.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/gsoomxfyz.sHtML

[R14] C 风格 for
来源：http://wap.fehbvm.com/Article/details/glptrykar.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/gmsvnlyeu.sHtML

[R15] while 逐行读文件
来源：http://wap.hesvh.cn/Article/details/gwbwonizo.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fehbvm.com/Article/details/grlxxqvkb.sHtML

[R16] until 等待条件
来源：http://blog.hesvh.cn/Article/details/gmhchulsm.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/gxwhbdfpz.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.hesvh.cn/Article/details/ghagsnceh.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.zdbjq.cn/Article/details/gxiezciir.sHtML

[R18] 遍历数组
来源：http://blog.zdbjq.cn/Article/details/gevoknres.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.zdbjq.cn/Article/details/ghxxwpgrh.sHtML

[R19] 数组长度
来源：http://baike.fehbvm.com/Article/details/gcdewehhw.sHtML

echo "${#arr[@]}"
来源：http://baike.fehbvm.com/Article/details/gkyxvadlx.sHtML

[R20] 关联数组（字典）
来源：http://read.share.zdbjq.cn/Article/details/gunjpdcpt.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fehbvm.com/Article/details/gzrefpfqv.sHtML

[R21] 字符串长度
来源：http://3g.fehbvm.com/Article/details/gqnwujiod.sHtML

echo "${#s}"
来源：http://blog.fehbvm.com/Article/details/giicudixi.sHtML

[R22] 截取子串
来源：http://3g.zdbjq.cn/Article/details/ggscqquxd.sHtML

echo "${s:0:5}"
来源：http://read.share.hesvh.cn/Article/details/gafwofkqn.sHtML

[R23] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/gqybknqxv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fehbvm.com/Article/details/gmohpzgae.sHtML

[R24] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gzyhrhrnq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.hesvh.cn/Article/details/gggtlvfbb.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.zdbjq.cn/Article/details/gylwggigg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.zdbjq.cn/Article/details/gibtqtqip.sHtML

[R26] 命令替换
来源：http://mobile.fehbvm.com/Article/details/gqehupxju.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.hesvh.cn/Article/details/gmbiyjntn.sHtML

[R27] 算术展开
来源：http://mobile.hesvh.cn/Article/details/gwmiehuxy.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.hesvh.cn/Article/details/gazbxqtpi.sHtML

[R28] 浮点运算
来源：http://www.m.share.zdbjq.cn/Article/details/gstpjhlnp.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.hesvh.cn/Article/details/goywajkbx.sHtML

[R29] 定义函数
来源：http://read.share.fehbvm.com/Article/details/gtxeitjht.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.hesvh.cn/Article/details/giwcuyxtp.sHtML

[R30] 函数返回状态码
来源：http://read.share.zdbjq.cn/Article/details/gmooqbbtd.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.zdbjq.cn/Article/details/glnedfxzv.sHtML

[R31] 局部变量
来源：http://m.share.fehbvm.com/Article/details/gasdfgdwp.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fehbvm.com/Article/details/gykfsiciv.sHtML

[R32] 参数个数校验
来源：http://blog.zdbjq.cn/Article/details/gtcglybzu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/ggknplrgg.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fehbvm.com/Article/details/grcdhnzsp.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.zdbjq.cn/Article/details/guqgbneor.sHtML

[R34] 退出时清理
来源：http://www.blog.fehbvm.com/Article/details/gkbkpbllv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gbollzdnd.sHtML

[R35] 后台执行并等待
来源：http://3g.hesvh.cn/Article/details/gdpgfrmtf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.hesvh.cn/Article/details/gnrahmhiq.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fehbvm.com/Article/details/gxymymdik.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.hesvh.cn/Article/details/gmtkmdjay.sHtML

[R37] 把输出赋给变量
来源：http://wap.fehbvm.com/Article/details/gxtghkewe.sHtML

files=$(ls -1)
来源：http://m.share.fehbvm.com/Article/details/gxameqqga.sHtML

[R38] 管道串联
来源：http://m.share.hesvh.cn/Article/details/gtezqdopb.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.hesvh.cn/Article/details/gocczqech.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.zdbjq.cn/Article/details/gmbbtmdma.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gqneojtwn.sHtML

[R40] 追加写日志
来源：http://www.share.fehbvm.com/Article/details/gvduigmsu.sHtML

echo "log" >> out.log
来源：http://read.share.fehbvm.com/Article/details/gzuibcunf.sHtML

[R41] 丢弃输出
来源：http://m.share.fehbvm.com/Article/details/guoacmkzu.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fehbvm.com/Article/details/gnpvvqgan.sHtML

[R42] 输入重定向
来源：http://wap.zdbjq.cn/Article/details/gpvazvkpk.sHtML

wc -l < a.txt
来源：http://www.share.fehbvm.com/Article/details/glkodqgwk.sHtML

[R43] 按名字查找文件
来源：http://wap.fehbvm.com/Article/details/gsnfpagjd.sHtML

find . -name "*.log" -type f
来源：http://baike.fehbvm.com/Article/details/grlzicxik.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fehbvm.com/Article/details/gypsgccun.sHtML

find . -mtime -7 -type f
来源：http://m.share.zdbjq.cn/Article/details/gwyycmudx.sHtML

[R45] 批量删除
来源：http://www.share.fehbvm.com/Article/details/gyzbiwesc.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.zdbjq.cn/Article/details/gqhtmuomd.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fehbvm.com/Article/details/gkraofavr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.zdbjq.cn/Article/details/gvljvqkap.sHtML

[R47] sed 单行替换
来源：http://read.share.fehbvm.com/Article/details/ggwujpheo.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gzxpkhfcd.sHtML

[R48] awk 取指定列
来源：http://blog.zdbjq.cn/Article/details/gboffwevz.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fehbvm.com/Article/details/ghbpvzvfi.sHtML

[R49] awk 带条件
来源：http://blog.zdbjq.cn/Article/details/gqjpkmqwq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.zdbjq.cn/Article/details/gxzkdrkfk.sHtML

[R50] awk 求和
来源：http://read.share.zdbjq.cn/Article/details/giigsmnoo.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gkycjevyf.sHtML

[R51] 排序去重取前几
来源：http://read.share.fehbvm.com/Article/details/gmnmxbbim.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fehbvm.com/Article/details/gpaqhpjxf.sHtML

[R52] 统计行数
来源：http://wap.hesvh.cn/Article/details/gjtpnsqeq.sHtML

wc -l a.txt
来源：http://3g.hesvh.cn/Article/details/gqkajxnvo.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.hesvh.cn/Article/details/gasoaxiso.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fehbvm.com/Article/details/gsuvkebnk.sHtML

[R54] 比较两个文件
来源：http://www.share.hesvh.cn/Article/details/gpntgrqqb.sHtML

diff a.txt b.txt
来源：http://m.share.zdbjq.cn/Article/details/gidsrqykn.sHtML

[R55] 压缩与解压
来源：http://wap.zdbjq.cn/Article/details/gqjhvjlum.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fehbvm.com/Article/details/ghlpqgiyd.sHtML

[R56] 远程拷贝
来源：http://read.share.fehbvm.com/Article/details/grtlhzpfd.sHtML

scp file user@host:/path/
来源：http://baike.fehbvm.com/Article/details/ghjrrsfkm.sHtML

[R57] 远程执行命令
来源：http://baike.hesvh.cn/Article/details/gyvccxsya.sHtML

ssh user@host 'uptime'
来源：http://m.share.fehbvm.com/Article/details/gvudfrzxa.sHtML

[R58] 下载文件
来源：http://www.share.hesvh.cn/Article/details/gmsagjbgg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.hesvh.cn/Article/details/gcjwaouci.sHtML

[R59] 发 POST JSON
来源：http://wap.fehbvm.com/Article/details/gyzspirxm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fehbvm.com/Article/details/gefybsksi.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/gokeijttr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fehbvm.com/Article/details/gbxtpovwg.sHtML

[R61] 磁盘占用
来源：http://www.blog.hesvh.cn/Article/details/gqqjaeggh.sHtML

df -h;  du -sh *
来源：http://m.share.zdbjq.cn/Article/details/gyusosses.sHtML

[R62] 找最占空间的文件
来源：http://www.share.zdbjq.cn/Article/details/gnexsjcyh.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fehbvm.com/Article/details/gpvylxpjn.sHtML

[R63] 内存与进程
来源：http://www.blog.fehbvm.com/Article/details/gvjsjefzs.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.hesvh.cn/Article/details/gfcmsvvby.sHtML

[R64] 结束进程
来源：http://www.blog.zdbjq.cn/Article/details/gbqopenex.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.zdbjq.cn/Article/details/gyqxzfjex.sHtML

[R65] 查看端口占用
来源：http://m.share.fehbvm.com/Article/details/gmxjrmzdn.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.zdbjq.cn/Article/details/guepiurmr.sHtML

[R66] 定时任务
来源：http://www.blog.fehbvm.com/Article/details/gxwrqcirx.sHtML

crontab -e;  crontab -l
来源：http://read.share.fehbvm.com/Article/details/ghfgiknzj.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.hesvh.cn/Article/details/gcvkqhatb.sHtML

openssl rand -hex 16
来源：http://read.share.zdbjq.cn/Article/details/gbjxfcbai.sHtML

[R68] 计算文件校验值
来源：http://3g.fehbvm.com/Article/details/gbbadakym.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fehbvm.com/Article/details/gkhsauweb.sHtML

[R69] 生成随机密码
来源：http://3g.zdbjq.cn/Article/details/gpldlkmvt.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fehbvm.com/Article/details/gngpzblvg.sHtML

[R70] 时间戳与互转
来源：http://baike.zdbjq.cn/Article/details/gtmiqwohf.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.zdbjq.cn/Article/details/grfqjumtf.sHtML

[R71] 日期格式化
来源：http://wap.fehbvm.com/Article/details/gsczhhecl.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.hesvh.cn/Article/details/gfpdhxihj.sHtML

[R72] 等待端口就绪
来源：http://www.blog.hesvh.cn/Article/details/gkcoeojmz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/gpfcappkt.sHtML

[R73] 分割大日志
来源：http://www.blog.zdbjq.cn/Article/details/gziqihxtk.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fehbvm.com/Article/details/gjitsmagh.sHtML

[R74] 批量重命名
来源：http://mobile.hesvh.cn/Article/details/gmubusopp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fehbvm.com/Article/details/gkqebggmd.sHtML

[R75] 导出环境变量
来源：http://read.share.hesvh.cn/Article/details/gtnnhqgpi.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fehbvm.com/Article/details/giyvcyiny.sHtML

[R76] 使用临时文件
来源：http://3g.fehbvm.com/Article/details/gxycoulcp.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/gttqoioap.sHtML

[R77] 读取用户输入
来源：http://3g.fehbvm.com/Article/details/gbbdkfmkl.sHtML

read -rp "请输入: " ans
来源：http://www.blog.zdbjq.cn/Article/details/gbzxwtfzf.sHtML

[R78] 交互式菜单
来源：http://3g.zdbjq.cn/Article/details/gdyrfdcdj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fehbvm.com/Article/details/ggkoazwsi.sHtML

[R79] 解析命令行选项
来源：http://3g.hesvh.cn/Article/details/gcowkjimb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fehbvm.com/Article/details/gqprbypoq.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.zdbjq.cn/Article/details/grhbkouln.sHtML

time ./run.sh
来源：http://www.share.zdbjq.cn/Article/details/gslagiqjt.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gmbysyjid.sHtML

S. C / C++ 专题
来源：http://3g.zdbjq.cn/Article/details/gukmtokwb.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gadqmizcm.sHtML

[S01] C：Hello World
来源：http://m.share.fehbvm.com/Article/details/gxfyfdjei.sHtML

#include <stdio.h>
来源：http://baike.hesvh.cn/Article/details/ghrsevdoh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.hesvh.cn/Article/details/gezrnobdc.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.zdbjq.cn/Article/details/gliydjnri.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fehbvm.com/Article/details/gnsthjrfc.sHtML

[S03] C：读入整数
来源：http://baike.zdbjq.cn/Article/details/gcgptrjsw.sHtML

int x; scanf("%d", &x);
来源：http://3g.fehbvm.com/Article/details/gngvfsrfr.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fehbvm.com/Article/details/ggalyiocc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.zdbjq.cn/Article/details/ggshkggcr.sHtML

[S05] C：字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gyqhqaabg.sHtML

strlen(s)
来源：http://wap.fehbvm.com/Article/details/grawgrlft.sHtML

[S06] C：字符串比较
来源：http://3g.hesvh.cn/Article/details/gvbosryip.sHtML

strcmp(a, b) == 0
来源：http://m.share.zdbjq.cn/Article/details/gvxtvmeaw.sHtML

[S07] C：数组遍历求和
来源：http://read.share.zdbjq.cn/Article/details/ginmmfxwr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.zdbjq.cn/Article/details/ghgytiroj.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.zdbjq.cn/Article/details/ghaubwtow.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.hesvh.cn/Article/details/gwvjuayqw.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.hesvh.cn/Article/details/gcqqnfoha.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.hesvh.cn/Article/details/gaickahue.sHtML

[S10] C：指针与解引用
来源：http://www.share.hesvh.cn/Article/details/gepdunwzv.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fehbvm.com/Article/details/grtqvpedd.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/glykezqfq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.hesvh.cn/Article/details/ghzcsknsx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.hesvh.cn/Article/details/gukynrwvn.sHtML

fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/golxyakal.sHtML

[S12] C：写文件
来源：http://www.blog.zdbjq.cn/Article/details/gcenifanl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.hesvh.cn/Article/details/gbwfyahid.sHtML

[S13] C：宏定义
来源：http://m.share.fehbvm.com/Article/details/gyihqxrok.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.hesvh.cn/Article/details/glchtjqbm.sHtML

[S14] C：枚举
来源：http://www.share.hesvh.cn/Article/details/gekaezgyg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.zdbjq.cn/Article/details/gbumjmeea.sHtML

[S15] C：类型转换
来源：http://read.share.hesvh.cn/Article/details/gndnstjsy.sHtML

(double) a / b
来源：http://m.share.zdbjq.cn/Article/details/gghnftrns.sHtML

[S16] C：位操作置位
来源：http://blog.hesvh.cn/Article/details/gbtysleph.sHtML

x |= (1 << 3);
来源：http://www.blog.fehbvm.com/Article/details/gmogdlvzn.sHtML

[S17] C：安全拼接字符串
来源：http://wap.hesvh.cn/Article/details/gkkdqlzuk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.zdbjq.cn/Article/details/gqexrpjvw.sHtML

[S18] C：命令行参数
来源：http://www.share.fehbvm.com/Article/details/glrhhholk.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.zdbjq.cn/Article/details/gbjncvhvn.sHtML

[S19] C：快速排序
来源：http://baike.hesvh.cn/Article/details/gkucrkhsi.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/gurzxiyzl.sHtML

[S20] C：二分查找
来源：http://baike.zdbjq.cn/Article/details/gmltpmptz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/gqfbekpzk.sHtML

[S21] C：字符类别判断
来源：http://mobile.hesvh.cn/Article/details/gdiyuaovf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.hesvh.cn/Article/details/gevotjlwz.sHtML

[S22] C：字符串转数字
来源：http://www.blog.hesvh.cn/Article/details/goonehwkm.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.hesvh.cn/Article/details/gdttgatwj.sHtML

[S23] C：随机数
来源：http://read.share.zdbjq.cn/Article/details/gwxrewozs.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.zdbjq.cn/Article/details/gzwkcnuny.sHtML

[S24] C：获取本地时间
来源：http://baike.hesvh.cn/Article/details/gkiaeutjc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fehbvm.com/Article/details/ghcetqyey.sHtML

[S25] C：内存拷贝
来源：http://m.share.hesvh.cn/Article/details/gyovlmlct.sHtML

memcpy(dst, src, n);
来源：http://blog.zdbjq.cn/Article/details/ggrfongbh.sHtML

[S26] C：内存清零
来源：http://baike.fehbvm.com/Article/details/gfqnyovlj.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fehbvm.com/Article/details/grqwgpser.sHtML

[S27] C：定义常量
来源：http://baike.zdbjq.cn/Article/details/gexoexrdl.sHtML

const double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gypoypozn.sHtML

[S28] C：静态变量
来源：http://read.share.fehbvm.com/Article/details/gowhozgak.sHtML

static int counter = 0;
来源：http://mobile.fehbvm.com/Article/details/gqenvqvxk.sHtML

[S29] C：变参函数
来源：http://read.share.fehbvm.com/Article/details/gowapaqch.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.hesvh.cn/Article/details/grranpwte.sHtML

[S30] C：头文件保护
来源：http://www.blog.hesvh.cn/Article/details/gjkmpaytb.sHtML

#ifndef X_H
来源：http://wap.zdbjq.cn/Article/details/gyvzxcsyl.sHtML

#define X_H
来源：http://wap.hesvh.cn/Article/details/gtkbslmxc.sHtML

#endif
来源：http://wap.zdbjq.cn/Article/details/gzzmgvnot.sHtML

[S31] C++：Hello World
来源：http://read.share.fehbvm.com/Article/details/gozkdbzfo.sHtML

#include <iostream>
来源：http://m.share.hesvh.cn/Article/details/grsfllaam.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.zdbjq.cn/Article/details/gzckakgav.sHtML

[S32] C++：字符串
来源：http://www.share.hesvh.cn/Article/details/grokaaqpv.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.hesvh.cn/Article/details/gkxnlikwx.sHtML

[S33] C++：vector 增删
来源：http://www.blog.hesvh.cn/Article/details/gyxurpxgi.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.zdbjq.cn/Article/details/gcrbjfdwg.sHtML

[S34] C++：遍历 vector
来源：http://m.share.hesvh.cn/Article/details/gurprmlel.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fehbvm.com/Article/details/gxqbvjdtv.sHtML

[S35] C++：map
来源：http://mobile.hesvh.cn/Article/details/gqbaefweu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/geyvwjupi.sHtML

[S36] C++：unordered_map
来源：http://www.share.zdbjq.cn/Article/details/gkrxzqmbz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/ghwqrboks.sHtML

[S37] C++：set
来源：http://m.share.fehbvm.com/Article/details/gznixvhdb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fehbvm.com/Article/details/gaghswfxr.sHtML

[S38] C++：排序
来源：http://3g.hesvh.cn/Article/details/gbiqtuebj.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.hesvh.cn/Article/details/gavpfuwcp.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fehbvm.com/Article/details/gmdkhhvpn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fehbvm.com/Article/details/gxynmcufz.sHtML

[S40] C++：查找元素
来源：http://read.share.zdbjq.cn/Article/details/glzzfzlqr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.hesvh.cn/Article/details/gbpootcfb.sHtML

[S41] C++：类与构造函数
来源：http://wap.hesvh.cn/Article/details/gjunvzfsj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.hesvh.cn/Article/details/gyqgrphjx.sHtML

[S42] C++：继承与虚函数
来源：http://blog.hesvh.cn/Article/details/gmuennpvg.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.zdbjq.cn/Article/details/gpvemxprt.sHtML

[S43] C++：智能指针
来源：http://baike.fehbvm.com/Article/details/gmnmiftml.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.hesvh.cn/Article/details/gjxvajozc.sHtML

[S44] C++：引用传参
来源：http://www.share.fehbvm.com/Article/details/gkmjoyzyq.sHtML

void inc(int &x) { ++x; }
来源：http://3g.zdbjq.cn/Article/details/gzbhdbqmp.sHtML

[S45] C++：lambda
来源：http://read.share.hesvh.cn/Article/details/gohcwfcjk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fehbvm.com/Article/details/ghugvlinn.sHtML

[S46] C++：函数模板
来源：http://mobile.hesvh.cn/Article/details/galnwueun.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.zdbjq.cn/Article/details/gjnmiclyz.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.hesvh.cn/Article/details/gpuxrnhyu.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.hesvh.cn/Article/details/gwkqhcqji.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gwxqspmtw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.zdbjq.cn/Article/details/gzskyweav.sHtML


<!-- 参考信息 -->