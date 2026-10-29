代发 wailian999

[Q80] 字符串截取
来源：http://baike.zdbjq.cn/Article/details/grwyjpbji.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gmhkqlmqp.sHtML

[Q81] 字符串替换
来源：http://baike.hesvh.cn/Article/details/goiyecste.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.hesvh.cn/Article/details/gopwegfta.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.hesvh.cn/Article/details/gvspqxmrd.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gkvdqxiqj.sHtML

[Q83] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/gnemjdcyx.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/ggjxjzjeg.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fehbvm.com/Article/details/gbtylcmjn.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gaidainmg.sHtML

[Q85] 数值取整
来源：http://www.m.share.hesvh.cn/Article/details/gdyifthhu.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.hesvh.cn/Article/details/gdmaqakdh.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.zdbjq.cn/Article/details/ghplhmeas.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fehbvm.com/Article/details/giybcycty.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.hesvh.cn/Article/details/gwersqmti.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fehbvm.com/Article/details/gqvaelsuf.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.hesvh.cn/Article/details/gtdnfqemq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.hesvh.cn/Article/details/gepehbdjz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fehbvm.com/Article/details/godeetfuq.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gkfwonbgg.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.zdbjq.cn/Article/details/ghpbnsfzh.sHtML

[Q90] 生成序号列
来源：http://wap.zdbjq.cn/Article/details/gbcckifzw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fehbvm.com/Article/details/gjbqyyrzu.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gormdjtwv.sHtML

R. Bash 专题
来源：http://www.blog.zdbjq.cn/Article/details/goebuzfet.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ghdjzmxdj.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fehbvm.com/Article/details/govebygdd.sHtML

#!/usr/bin/env bash
来源：http://read.share.hesvh.cn/Article/details/giuoirvkh.sHtML

set -euo pipefail
来源：http://www.blog.fehbvm.com/Article/details/givsjakyp.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fehbvm.com/Article/details/gtzcuamvx.sHtML

name="Tom"; echo "$name"
来源：http://wap.zdbjq.cn/Article/details/gloepbgyr.sHtML

[R03] 只读变量
来源：http://blog.zdbjq.cn/Article/details/gkmymaead.sHtML

readonly PI=3.14
来源：http://mobile.fehbvm.com/Article/details/glxzwdcpl.sHtML

[R04] 位置参数
来源：http://read.share.hesvh.cn/Article/details/gretlqytb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.zdbjq.cn/Article/details/ggneqefas.sHtML

[R05] 参数默认值
来源：http://mobile.fehbvm.com/Article/details/gaismxwun.sHtML

name="${1:-default}"
来源：http://m.share.zdbjq.cn/Article/details/gutqjrrch.sHtML

[R06] 判断命令是否存在
来源：http://3g.hesvh.cn/Article/details/gpjteqlgs.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/gfnbiwkfm.sHtML

[R07] if 判断文件
来源：http://www.m.share.zdbjq.cn/Article/details/gbomemukr.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gdurlzalc.sHtML

[R08] 数值比较
来源：http://blog.fehbvm.com/Article/details/guycehobh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.zdbjq.cn/Article/details/gvrfzhnba.sHtML

[R09] 字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gjewvaoka.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.hesvh.cn/Article/details/gomjuwexi.sHtML

[R10] 正则匹配
来源：http://www.blog.hesvh.cn/Article/details/gajagnudf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.hesvh.cn/Article/details/gmfumlqfb.sHtML

[R11] case 多分支
来源：http://www.blog.zdbjq.cn/Article/details/ggancxtep.sHtML

case "$1" in
来源：http://mobile.hesvh.cn/Article/details/giwnfvqac.sHtML

start) echo "启动" ;;
来源：http://m.share.zdbjq.cn/Article/details/gbbtvapgg.sHtML

stop)  echo "停止" ;;
来源：http://m.share.hesvh.cn/Article/details/guvffnidu.sHtML

*)     echo "未知命令" ;;
来源：http://3g.hesvh.cn/Article/details/glwlnaudb.sHtML

esac
来源：http://mobile.hesvh.cn/Article/details/gdmjswcpi.sHtML

[R12] for 遍历文件
来源：http://wap.zdbjq.cn/Article/details/gunvpzxqs.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.zdbjq.cn/Article/details/gqlkugkar.sHtML

[R13] for 计数循环
来源：http://wap.fehbvm.com/Article/details/ggcrsebbk.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/grclttqmm.sHtML

[R14] C 风格 for
来源：http://3g.zdbjq.cn/Article/details/gpxnbocrh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/gswejwhgi.sHtML

[R15] while 逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gtlqfuthk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.zdbjq.cn/Article/details/ghitoggig.sHtML

[R16] until 等待条件
来源：http://read.share.zdbjq.cn/Article/details/gzdgebabx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/gydbpqsad.sHtML

[R17] 数组定义与取值
来源：http://m.share.fehbvm.com/Article/details/gizgzcxaz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.zdbjq.cn/Article/details/gtrgmzgrx.sHtML

[R18] 遍历数组
来源：http://mobile.fehbvm.com/Article/details/glbowewbq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.zdbjq.cn/Article/details/gancwkkig.sHtML

[R19] 数组长度
来源：http://m.share.hesvh.cn/Article/details/gadkvgasc.sHtML

echo "${#arr[@]}"
来源：http://m.share.hesvh.cn/Article/details/gahzmxqit.sHtML

[R20] 关联数组（字典）
来源：http://3g.fehbvm.com/Article/details/gxbmfsimv.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.hesvh.cn/Article/details/gmzgtrona.sHtML

[R21] 字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gneucjksn.sHtML

echo "${#s}"
来源：http://www.blog.fehbvm.com/Article/details/gffpotsdi.sHtML

[R22] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/gwbmctbii.sHtML

echo "${s:0:5}"
来源：http://www.share.zdbjq.cn/Article/details/gdovqvjnv.sHtML

[R23] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/gntpapjza.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fehbvm.com/Article/details/gudwhokax.sHtML

[R24] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gkwhbgmov.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.hesvh.cn/Article/details/gtfffschq.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fehbvm.com/Article/details/gnjvlmnzp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.hesvh.cn/Article/details/gurruxbav.sHtML

[R26] 命令替换
来源：http://www.m.share.fehbvm.com/Article/details/gjkerwszj.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.zdbjq.cn/Article/details/gxxzphbfh.sHtML

[R27] 算术展开
来源：http://www.m.share.hesvh.cn/Article/details/gglnbfggm.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.hesvh.cn/Article/details/grzifoosj.sHtML

[R28] 浮点运算
来源：http://3g.fehbvm.com/Article/details/guyauisbj.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fehbvm.com/Article/details/grybzitly.sHtML

[R29] 定义函数
来源：http://read.share.zdbjq.cn/Article/details/gsctcolpc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.hesvh.cn/Article/details/grlydnckj.sHtML

[R30] 函数返回状态码
来源：http://m.share.zdbjq.cn/Article/details/goqyyhyox.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fehbvm.com/Article/details/gyiurubrk.sHtML

[R31] 局部变量
来源：http://wap.hesvh.cn/Article/details/gqlotuyfm.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.hesvh.cn/Article/details/gjzquenep.sHtML

[R32] 参数个数校验
来源：http://www.blog.fehbvm.com/Article/details/ggiohexgg.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/grztpmglz.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fehbvm.com/Article/details/gqvmspknl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.zdbjq.cn/Article/details/gdfccbpuo.sHtML

[R34] 退出时清理
来源：http://m.share.fehbvm.com/Article/details/gyhojnfii.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gyzwmdcbz.sHtML

[R35] 后台执行并等待
来源：http://mobile.fehbvm.com/Article/details/gufftices.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.hesvh.cn/Article/details/gmpyoysmh.sHtML

[R36] 并发执行多个任务
来源：http://blog.fehbvm.com/Article/details/gjxviuokr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.hesvh.cn/Article/details/gdujszkku.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.hesvh.cn/Article/details/gnlinmpjj.sHtML

files=$(ls -1)
来源：http://www.blog.hesvh.cn/Article/details/gvhrewwgn.sHtML

[R38] 管道串联
来源：http://m.share.fehbvm.com/Article/details/gxkoodzir.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.zdbjq.cn/Article/details/gmhwxsqdd.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.zdbjq.cn/Article/details/gnekmruok.sHtML

cmd > out.log 2>&1
来源：http://wap.fehbvm.com/Article/details/gtvvwoyhe.sHtML

[R40] 追加写日志
来源：http://read.share.hesvh.cn/Article/details/gyivdvjgt.sHtML

echo "log" >> out.log
来源：http://3g.fehbvm.com/Article/details/gvakqnhsl.sHtML

[R41] 丢弃输出
来源：http://mobile.hesvh.cn/Article/details/glqxletqp.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/grwglnczj.sHtML

[R42] 输入重定向
来源：http://read.share.zdbjq.cn/Article/details/gzycqwgoh.sHtML

wc -l < a.txt
来源：http://baike.zdbjq.cn/Article/details/geyzknfmq.sHtML

[R43] 按名字查找文件
来源：http://mobile.zdbjq.cn/Article/details/gecraybbm.sHtML

find . -name "*.log" -type f
来源：http://wap.fehbvm.com/Article/details/gneumdxxy.sHtML

[R44] 按修改时间查找
来源：http://m.share.hesvh.cn/Article/details/gdpovrrsf.sHtML

find . -mtime -7 -type f
来源：http://read.share.zdbjq.cn/Article/details/gudhkpokm.sHtML

[R45] 批量删除
来源：http://www.share.fehbvm.com/Article/details/giqsdgnub.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.hesvh.cn/Article/details/gkpbbsiuj.sHtML

[R46] 递归替换文件内容
来源：http://read.share.hesvh.cn/Article/details/gljzsipnm.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fehbvm.com/Article/details/givuxgtoz.sHtML

[R47] sed 单行替换
来源：http://wap.fehbvm.com/Article/details/gatxmjrjf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.hesvh.cn/Article/details/gtxeztedk.sHtML

[R48] awk 取指定列
来源：http://www.blog.zdbjq.cn/Article/details/gufgmxcyh.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.hesvh.cn/Article/details/gbebepcaj.sHtML

[R49] awk 带条件
来源：http://read.share.hesvh.cn/Article/details/gjjhgddcv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fehbvm.com/Article/details/gemttffnb.sHtML

[R50] awk 求和
来源：http://read.share.fehbvm.com/Article/details/gfzcmrjij.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gcnhyzowc.sHtML

[R51] 排序去重取前几
来源：http://3g.zdbjq.cn/Article/details/gndlfoscp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.zdbjq.cn/Article/details/grfhwiajv.sHtML

[R52] 统计行数
来源：http://m.share.fehbvm.com/Article/details/gyefacyzr.sHtML

wc -l a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gtwrohcgm.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.hesvh.cn/Article/details/gbvcuppcj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.zdbjq.cn/Article/details/ghxnrljlq.sHtML

[R54] 比较两个文件
来源：http://3g.hesvh.cn/Article/details/gpecyvmba.sHtML

diff a.txt b.txt
来源：http://baike.zdbjq.cn/Article/details/gthysbxiw.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fehbvm.com/Article/details/gpzwsazjo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fehbvm.com/Article/details/gnksfzluk.sHtML

[R56] 远程拷贝
来源：http://3g.hesvh.cn/Article/details/gwluqyxyy.sHtML

scp file user@host:/path/
来源：http://www.blog.hesvh.cn/Article/details/gnorhttzg.sHtML

[R57] 远程执行命令
来源：http://m.share.hesvh.cn/Article/details/gkdfnrbvy.sHtML

ssh user@host 'uptime'
来源：http://baike.hesvh.cn/Article/details/glsebpgbc.sHtML

[R58] 下载文件
来源：http://read.share.hesvh.cn/Article/details/glocwtsmb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.hesvh.cn/Article/details/gifbuwpqi.sHtML

[R59] 发 POST JSON
来源：http://www.share.zdbjq.cn/Article/details/gzwbuvkxc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fehbvm.com/Article/details/gidgpcxay.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.hesvh.cn/Article/details/gcxrgazvy.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.zdbjq.cn/Article/details/gqfzymkzo.sHtML

[R61] 磁盘占用
来源：http://wap.fehbvm.com/Article/details/gnkzgnqan.sHtML

df -h;  du -sh *
来源：http://www.share.hesvh.cn/Article/details/gslvxvpdc.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fehbvm.com/Article/details/gdqfmeazc.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.zdbjq.cn/Article/details/gneuhqbqj.sHtML

[R63] 内存与进程
来源：http://www.share.zdbjq.cn/Article/details/gqnbqossg.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.zdbjq.cn/Article/details/gmlcojyrn.sHtML

[R64] 结束进程
来源：http://www.share.hesvh.cn/Article/details/gbklsvsdv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.hesvh.cn/Article/details/glghcczii.sHtML

[R65] 查看端口占用
来源：http://www.m.share.hesvh.cn/Article/details/gbetyqhej.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fehbvm.com/Article/details/gufmfuidu.sHtML

[R66] 定时任务
来源：http://read.share.zdbjq.cn/Article/details/gpaffsjos.sHtML

crontab -e;  crontab -l
来源：http://mobile.hesvh.cn/Article/details/gekdnispu.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fehbvm.com/Article/details/gnvrxeyvx.sHtML

openssl rand -hex 16
来源：http://www.m.share.hesvh.cn/Article/details/gwljtobfd.sHtML

[R68] 计算文件校验值
来源：http://m.share.zdbjq.cn/Article/details/gzobpiypl.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gpnqokoma.sHtML

[R69] 生成随机密码
来源：http://wap.hesvh.cn/Article/details/gjempenec.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.hesvh.cn/Article/details/gikougneg.sHtML

[R70] 时间戳与互转
来源：http://m.share.zdbjq.cn/Article/details/ggaioyoac.sHtML

date +%s;  date -d @1700000000
来源：http://baike.hesvh.cn/Article/details/grqsahiiy.sHtML

[R71] 日期格式化
来源：http://baike.fehbvm.com/Article/details/gcnoawzmt.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fehbvm.com/Article/details/gzxbyiuua.sHtML

[R72] 等待端口就绪
来源：http://wap.fehbvm.com/Article/details/gspshbtcn.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/gpwhcjbmz.sHtML

[R73] 分割大日志
来源：http://read.share.hesvh.cn/Article/details/gluelzdrw.sHtML

split -l 1000 big.log part_
来源：http://mobile.hesvh.cn/Article/details/gmfxdudes.sHtML

[R74] 批量重命名
来源：http://baike.fehbvm.com/Article/details/gfujwvaek.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.zdbjq.cn/Article/details/gzsiqfvum.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fehbvm.com/Article/details/ggdpydxvk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.zdbjq.cn/Article/details/gzqhbrwmz.sHtML

[R76] 使用临时文件
来源：http://mobile.zdbjq.cn/Article/details/gpcxhqwps.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/gdizsqvnb.sHtML

[R77] 读取用户输入
来源：http://m.share.zdbjq.cn/Article/details/gktvvkelz.sHtML

read -rp "请输入: " ans
来源：http://www.blog.zdbjq.cn/Article/details/ghuxqwray.sHtML

[R78] 交互式菜单
来源：http://mobile.hesvh.cn/Article/details/gyjfkivgh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.hesvh.cn/Article/details/gbhlhbtks.sHtML

[R79] 解析命令行选项
来源：http://wap.fehbvm.com/Article/details/gwgusxqrr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.zdbjq.cn/Article/details/gkudlarhl.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.zdbjq.cn/Article/details/gyrrrnjxd.sHtML

time ./run.sh
来源：http://www.blog.fehbvm.com/Article/details/gjmlioaav.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gfpalonjw.sHtML

S. C / C++ 专题
来源：http://baike.fehbvm.com/Article/details/gcmrxkhdp.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gicoozhqk.sHtML

[S01] C：Hello World
来源：http://blog.fehbvm.com/Article/details/gmploznue.sHtML

#include <stdio.h>
来源：http://baike.fehbvm.com/Article/details/ghcvtsnnp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.zdbjq.cn/Article/details/grnppjpje.sHtML

[S02] C：变量与格式化输出
来源：http://blog.zdbjq.cn/Article/details/gkkzvjawm.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.zdbjq.cn/Article/details/gpnoripfv.sHtML

[S03] C：读入整数
来源：http://www.blog.hesvh.cn/Article/details/gedsgvoad.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.hesvh.cn/Article/details/ghslkpysz.sHtML

[S04] C：字符串复制
来源：http://m.share.fehbvm.com/Article/details/gxmdrebbm.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.zdbjq.cn/Article/details/gmrtbhqye.sHtML

[S05] C：字符串长度
来源：http://read.share.hesvh.cn/Article/details/gijicjsez.sHtML

strlen(s)
来源：http://www.share.hesvh.cn/Article/details/gaxzxmlkz.sHtML

[S06] C：字符串比较
来源：http://mobile.fehbvm.com/Article/details/gqxrosjfv.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.zdbjq.cn/Article/details/gagvryhys.sHtML

[S07] C：数组遍历求和
来源：http://blog.fehbvm.com/Article/details/gxqvlatzr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.hesvh.cn/Article/details/gzgsabekz.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.hesvh.cn/Article/details/gygaqszsz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.hesvh.cn/Article/details/gimlvqowz.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.hesvh.cn/Article/details/gbtalhavg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fehbvm.com/Article/details/gxtjppurc.sHtML

[S10] C：指针与解引用
来源：http://baike.hesvh.cn/Article/details/gpkfvtrgu.sHtML

int *p = &a;  *p = 5;
来源：http://wap.zdbjq.cn/Article/details/glistroup.sHtML

[S11] C：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gdqdweyxc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.hesvh.cn/Article/details/gbixiwwks.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.zdbjq.cn/Article/details/gnzhtagnc.sHtML

fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/gfoinebgg.sHtML

[S12] C：写文件
来源：http://read.share.zdbjq.cn/Article/details/gqfxnqqvi.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fehbvm.com/Article/details/gjwjmegcl.sHtML

[S13] C：宏定义
来源：http://blog.zdbjq.cn/Article/details/gsgoxsjmi.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fehbvm.com/Article/details/gazzvkmqm.sHtML

[S14] C：枚举
来源：http://wap.fehbvm.com/Article/details/goksyehvl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.hesvh.cn/Article/details/gliyahgax.sHtML

[S15] C：类型转换
来源：http://mobile.zdbjq.cn/Article/details/gfdewubsz.sHtML

(double) a / b
来源：http://m.share.fehbvm.com/Article/details/gauqnyocg.sHtML

[S16] C：位操作置位
来源：http://read.share.zdbjq.cn/Article/details/gqynilfcd.sHtML

x |= (1 << 3);
来源：http://read.share.hesvh.cn/Article/details/glxnflfjz.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gpbyhmqkh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.zdbjq.cn/Article/details/gjsnqbqcw.sHtML

[S18] C：命令行参数
来源：http://mobile.fehbvm.com/Article/details/gdbqzazrl.sHtML

int main(int argc, char **argv)
来源：http://m.share.hesvh.cn/Article/details/gdhplfsos.sHtML

[S19] C：快速排序
来源：http://m.share.fehbvm.com/Article/details/gtbkfmnuo.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gnlhqgafb.sHtML

[S20] C：二分查找
来源：http://mobile.fehbvm.com/Article/details/gbjvdsinr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gonqpgtgz.sHtML

[S21] C：字符类别判断
来源：http://blog.zdbjq.cn/Article/details/gsftqorcl.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fehbvm.com/Article/details/gkjyfpect.sHtML

[S22] C：字符串转数字
来源：http://wap.fehbvm.com/Article/details/ghzcgizmn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.zdbjq.cn/Article/details/gepppxthh.sHtML

[S23] C：随机数
来源：http://www.share.fehbvm.com/Article/details/gexrrqcct.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.hesvh.cn/Article/details/gfrkjmdjd.sHtML

[S24] C：获取本地时间
来源：http://baike.zdbjq.cn/Article/details/gonuaeuhc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.hesvh.cn/Article/details/gpfjndjpl.sHtML

[S25] C：内存拷贝
来源：http://baike.hesvh.cn/Article/details/gyyhnfxnq.sHtML

memcpy(dst, src, n);
来源：http://read.share.fehbvm.com/Article/details/gfpxovuhe.sHtML

[S26] C：内存清零
来源：http://www.share.hesvh.cn/Article/details/gulidjfua.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fehbvm.com/Article/details/gvlztzvfk.sHtML

[S27] C：定义常量
来源：http://www.m.share.zdbjq.cn/Article/details/gcugbdzme.sHtML

const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gygwctdtq.sHtML

[S28] C：静态变量
来源：http://blog.hesvh.cn/Article/details/gazjpvmvj.sHtML

static int counter = 0;
来源：http://www.m.share.hesvh.cn/Article/details/gbyaajzwy.sHtML

[S29] C：变参函数
来源：http://read.share.zdbjq.cn/Article/details/gprzztfiv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.hesvh.cn/Article/details/gntcxvalf.sHtML

[S30] C：头文件保护
来源：http://mobile.fehbvm.com/Article/details/gfgyermtb.sHtML

#ifndef X_H
来源：http://3g.fehbvm.com/Article/details/ggcgnlrts.sHtML

#define X_H
来源：http://wap.zdbjq.cn/Article/details/gofsocspz.sHtML

#endif
来源：http://blog.fehbvm.com/Article/details/grlakxmkn.sHtML

[S31] C++：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gyyzffyrj.sHtML

#include <iostream>
来源：http://www.share.hesvh.cn/Article/details/gqnzfmezz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.hesvh.cn/Article/details/gcyqqzbgs.sHtML

[S32] C++：字符串
来源：http://m.share.fehbvm.com/Article/details/ghdmmjpjj.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.zdbjq.cn/Article/details/glvrhwiml.sHtML

[S33] C++：vector 增删
来源：http://read.share.zdbjq.cn/Article/details/gapdkotmh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.hesvh.cn/Article/details/grauvsxzs.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fehbvm.com/Article/details/gwlwywcxq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.hesvh.cn/Article/details/gsgydtkey.sHtML

[S35] C++：map
来源：http://read.share.fehbvm.com/Article/details/gtoxowgds.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gtesfztlv.sHtML

[S36] C++：unordered_map
来源：http://m.share.fehbvm.com/Article/details/glwplvtsc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gncljrevz.sHtML

[S37] C++：set
来源：http://baike.hesvh.cn/Article/details/gwonaencl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.zdbjq.cn/Article/details/gwzjwbsrs.sHtML

[S38] C++：排序
来源：http://www.share.zdbjq.cn/Article/details/giajpvxxq.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.zdbjq.cn/Article/details/goeaqhmnb.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.zdbjq.cn/Article/details/gxldmcuri.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fehbvm.com/Article/details/gbdnbumev.sHtML

[S40] C++：查找元素
来源：http://read.share.hesvh.cn/Article/details/gjsqunyvm.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.zdbjq.cn/Article/details/gfnjsjmpx.sHtML

[S41] C++：类与构造函数
来源：http://mobile.hesvh.cn/Article/details/gdbxcjxid.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.zdbjq.cn/Article/details/gkbdzrxhj.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fehbvm.com/Article/details/grdaeoxsb.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fehbvm.com/Article/details/gbhbdwwad.sHtML

[S43] C++：智能指针
来源：http://m.share.hesvh.cn/Article/details/gujbdudxx.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.zdbjq.cn/Article/details/gtrvqoqqc.sHtML

[S44] C++：引用传参
来源：http://3g.fehbvm.com/Article/details/goxtrcijj.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkbhinlen.sHtML

[S45] C++：lambda
来源：http://mobile.zdbjq.cn/Article/details/gdiqterau.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fehbvm.com/Article/details/gyxmtdafb.sHtML

[S46] C++：函数模板
来源：http://www.m.share.hesvh.cn/Article/details/gtfbwexpg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.hesvh.cn/Article/details/gqxchffkz.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.hesvh.cn/Article/details/gycyzdtnt.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.hesvh.cn/Article/details/gahlfknks.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gxnjgjgsr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fehbvm.com/Article/details/gzdcyoezf.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.zdbjq.cn/Article/details/gflzhdihb.sHtML

[S49] C++：写文件
来源：http://www.blog.zdbjq.cn/Article/details/gjtjishse.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.hesvh.cn/Article/details/gnmksxlgh.sHtML

[S50] C++：格式化数字
来源：http://baike.zdbjq.cn/Article/details/gltyavdqk.sHtML


<!-- 参考信息 -->