代发 wailian999

[Q86] 读取 JSON 字段
来源：http://wap.fanxiaobao.xyz/Article/details/ganlqcqlq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fanxiaobao.xyz/Article/details/gctamvhbq.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gmjalazrz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fanxiaobao.xyz/Article/details/gyvacnqzy.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fanxiaobao.xyz/Article/details/gmlxvygwk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fanxiaobao.xyz/Article/details/gyglgvdts.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gtiuyanmc.sHtML

[Q89] 判断表是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gsryknhvx.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gfkwftqeg.sHtML

[Q90] 生成序号列
来源：http://www.share.fanxiaobao.xyz/Article/details/glnzmbhwb.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtsazqogv.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpsfzsbgc.sHtML

R. Bash 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gxujlcihb.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gzubduhpz.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fanxiaobao.xyz/Article/details/guqjyvgke.sHtML

#!/usr/bin/env bash
来源：http://mobile.fanxiaobao.xyz/Article/details/gffieixuo.sHtML

set -euo pipefail
来源：http://blog.fanxiaobao.xyz/Article/details/gtajnfwim.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwxjuwsd.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjvisrih.sHtML

[R03] 只读变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gtegyokdg.sHtML

readonly PI=3.14
来源：http://read.share.fanxiaobao.xyz/Article/details/gkgplbyqc.sHtML

[R04] 位置参数
来源：http://3g.fanxiaobao.xyz/Article/details/gujlmgbfi.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fanxiaobao.xyz/Article/details/gabjuqevr.sHtML

[R05] 参数默认值
来源：http://read.share.fanxiaobao.xyz/Article/details/gjmlmhycx.sHtML

name="${1:-default}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidzipypw.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/geczlvgzz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxeywtegs.sHtML

[R07] if 判断文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gonqjscam.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gcitamvfn.sHtML

[R08] 数值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/grwbimmsp.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbyajocu.sHtML

[R09] 字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gdnpcduwl.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/ghvsuelqc.sHtML

[R10] 正则匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gnowxmimx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/guvxncfdf.sHtML

[R11] case 多分支
来源：http://www.share.fanxiaobao.xyz/Article/details/gtuydtuqj.sHtML

case "$1" in
来源：http://www.share.fanxiaobao.xyz/Article/details/gplltuqdk.sHtML

start) echo "启动" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkjsllmcp.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfrudtlig.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gkattajxk.sHtML

esac
来源：http://baike.fanxiaobao.xyz/Article/details/gooovmyby.sHtML

[R12] for 遍历文件
来源：http://baike.fanxiaobao.xyz/Article/details/gylzcxpkw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gimtfyiyx.sHtML

[R13] for 计数循环
来源：http://wap.fanxiaobao.xyz/Article/details/gqxvcktcl.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gxdivrotf.sHtML

[R14] C 风格 for
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjfccdwx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmlcosvv.sHtML

[R15] while 逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gwsuzdyms.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gqvmvefwi.sHtML

[R16] until 等待条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpckdclrx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gsufwspug.sHtML

[R17] 数组定义与取值
来源：http://blog.fanxiaobao.xyz/Article/details/gbyxvqeie.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gzmanmcrd.sHtML

[R18] 遍历数组
来源：http://blog.fanxiaobao.xyz/Article/details/gvmanefus.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gafivnsda.sHtML

[R19] 数组长度
来源：http://wap.fanxiaobao.xyz/Article/details/garednema.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gztrrqwpy.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fanxiaobao.xyz/Article/details/galejuubg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gjwxpdfsg.sHtML

[R21] 字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gssepuqlk.sHtML

echo "${#s}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gjlurzhlp.sHtML

[R22] 截取子串
来源：http://baike.fanxiaobao.xyz/Article/details/gdezhbktz.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnsziupzb.sHtML

[R23] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gzltvvizq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fanxiaobao.xyz/Article/details/gxmdiqmml.sHtML

[R24] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gbiwdidpc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gobvquxkb.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/gocpoicdw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fanxiaobao.xyz/Article/details/gdkfqqrwo.sHtML

[R26] 命令替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbemsfubq.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzvynrjbs.sHtML

[R27] 算术展开
来源：http://blog.fanxiaobao.xyz/Article/details/gmarhnvuv.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fanxiaobao.xyz/Article/details/geoxsmmxd.sHtML

[R28] 浮点运算
来源：http://baike.fanxiaobao.xyz/Article/details/gpmcowrik.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbhzzbbzv.sHtML

[R29] 定义函数
来源：http://mobile.fanxiaobao.xyz/Article/details/geolbfoho.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gylgltcpa.sHtML

[R30] 函数返回状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gjavphhjz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzcxhvxzl.sHtML

[R31] 局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxyrxepup.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gxulnaexo.sHtML

[R32] 参数个数校验
来源：http://3g.fanxiaobao.xyz/Article/details/gklvpbmhr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gisdiorms.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gntzuipui.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fanxiaobao.xyz/Article/details/gzsoahhzz.sHtML

[R34] 退出时清理
来源：http://www.share.fanxiaobao.xyz/Article/details/gtvnpzafo.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcczqtfdq.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwkcjkwhy.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fanxiaobao.xyz/Article/details/gxjxmcbhi.sHtML

[R36] 并发执行多个任务
来源：http://wap.fanxiaobao.xyz/Article/details/gzgjtymoz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/gzekcztrw.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsatjyxhg.sHtML

files=$(ls -1)
来源：http://3g.fanxiaobao.xyz/Article/details/gqheskmes.sHtML

[R38] 管道串联
来源：http://read.share.fanxiaobao.xyz/Article/details/ggcuidkwq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gkskqezll.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmrjccme.sHtML

cmd > out.log 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gzqwfqjni.sHtML

[R40] 追加写日志
来源：http://3g.fanxiaobao.xyz/Article/details/gnewvbksx.sHtML

echo "log" >> out.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamwdjymj.sHtML

[R41] 丢弃输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggrempwai.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gkzjofzkw.sHtML

[R42] 输入重定向
来源：http://3g.fanxiaobao.xyz/Article/details/gjubdfiew.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqvrypyof.sHtML

[R43] 按名字查找文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gocifsuqz.sHtML

find . -name "*.log" -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gouorgwrh.sHtML

[R44] 按修改时间查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gtkegcbyi.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gvjajcmoz.sHtML

[R45] 批量删除
来源：http://blog.fanxiaobao.xyz/Article/details/gfrhzdufx.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fanxiaobao.xyz/Article/details/gyuokrtlu.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fanxiaobao.xyz/Article/details/gymlgcatb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fanxiaobao.xyz/Article/details/gsevaoxuz.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gglpguqxs.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkfxipvhy.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/gmedvqkzg.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/ggjhmsrnv.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gvyjrhmrn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmgfcdta.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gafigbozf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gyogkcqar.sHtML

[R51] 排序去重取前几
来源：http://wap.fanxiaobao.xyz/Article/details/gfigmkhki.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fanxiaobao.xyz/Article/details/gqjyaciza.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/gsyratpfy.sHtML

wc -l a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gompzbzpy.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fanxiaobao.xyz/Article/details/gwfsikeqm.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpxkqgcvs.sHtML

[R54] 比较两个文件
来源：http://3g.fanxiaobao.xyz/Article/details/giqtjmtbn.sHtML

diff a.txt b.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcjqqcrby.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/gqomeoahi.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fanxiaobao.xyz/Article/details/gghcfnbwe.sHtML

[R56] 远程拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gzpmlsshn.sHtML

scp file user@host:/path/
来源：http://www.share.fanxiaobao.xyz/Article/details/gxopmakvt.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/gneyujxtc.sHtML

ssh user@host 'uptime'
来源：http://baike.fanxiaobao.xyz/Article/details/gdgcvzpag.sHtML

[R58] 下载文件
来源：http://blog.fanxiaobao.xyz/Article/details/ganbjrash.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fanxiaobao.xyz/Article/details/gonprdbgo.sHtML

[R59] 发 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gngxhaotp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fanxiaobao.xyz/Article/details/gwsvzhxfa.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gtjvuflhz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gilufbuka.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggdwxtzdp.sHtML

df -h;  du -sh *
来源：http://mobile.fanxiaobao.xyz/Article/details/glohpianm.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjoibuzn.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fanxiaobao.xyz/Article/details/gsasqtsas.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/grozbbugg.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fanxiaobao.xyz/Article/details/gihtfpegg.sHtML

[R64] 结束进程
来源：http://blog.fanxiaobao.xyz/Article/details/gvudlxmfq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcpzhspfk.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdqvjsnex.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gerjpmwbk.sHtML

[R66] 定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gizwisjgg.sHtML

crontab -e;  crontab -l
来源：http://m.share.fanxiaobao.xyz/Article/details/ghukyohsn.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fanxiaobao.xyz/Article/details/guqnxduih.sHtML

openssl rand -hex 16
来源：http://wap.fanxiaobao.xyz/Article/details/glbpljnoh.sHtML

[R68] 计算文件校验值
来源：http://wap.fanxiaobao.xyz/Article/details/gkdfvvpxf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghhnwfgmg.sHtML

[R69] 生成随机密码
来源：http://www.blog.fanxiaobao.xyz/Article/details/giyrxlfjb.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fanxiaobao.xyz/Article/details/gwuxvlkzi.sHtML

[R70] 时间戳与互转
来源：http://baike.fanxiaobao.xyz/Article/details/gpvnrjwxu.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyzwggjgc.sHtML

[R71] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/guawafudp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fanxiaobao.xyz/Article/details/goinojpdu.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gralddouf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gyeagbhtp.sHtML

[R73] 分割大日志
来源：http://wap.fanxiaobao.xyz/Article/details/gjmmegzqp.sHtML

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/gthjkjytr.sHtML

[R74] 批量重命名
来源：http://3g.fanxiaobao.xyz/Article/details/gbwxqysog.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gijhzuhxm.sHtML

[R75] 导出环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/grdijxuui.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fanxiaobao.xyz/Article/details/gbdxwqpvo.sHtML

[R76] 使用临时文件
来源：http://blog.fanxiaobao.xyz/Article/details/gynnaxjhi.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/grjglierx.sHtML

[R77] 读取用户输入
来源：http://blog.fanxiaobao.xyz/Article/details/gdmwoljsv.sHtML

read -rp "请输入: " ans
来源：http://mobile.fanxiaobao.xyz/Article/details/gyyprnyni.sHtML

[R78] 交互式菜单
来源：http://www.share.fanxiaobao.xyz/Article/details/gnhcgjzwq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/gsilzczht.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/gjndmwcqg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvtecyge.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fanxiaobao.xyz/Article/details/gmayfqjjr.sHtML

time ./run.sh
来源：http://m.share.fanxiaobao.xyz/Article/details/gpvzzmevk.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghgnohuor.sHtML

S. C / C++ 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gmafriqmd.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gmmkldmqg.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjriqfcvm.sHtML

#include <stdio.h>
来源：http://mobile.fanxiaobao.xyz/Article/details/gkrxcqdck.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fanxiaobao.xyz/Article/details/grjvhbkuo.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fanxiaobao.xyz/Article/details/gmmwadaur.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/gcpesvrua.sHtML

[S03] C：读入整数
来源：http://blog.fanxiaobao.xyz/Article/details/gacvqqxmd.sHtML

int x; scanf("%d", &x);
来源：http://baike.fanxiaobao.xyz/Article/details/gmdqlcosx.sHtML

[S04] C：字符串复制
来源：http://baike.fanxiaobao.xyz/Article/details/gkdnkydcz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/gxrhfzcmz.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/givdnfshx.sHtML

strlen(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghifvfitl.sHtML

[S06] C：字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gedogrdxb.sHtML

strcmp(a, b) == 0
来源：http://blog.fanxiaobao.xyz/Article/details/geyhlxyzu.sHtML

[S07] C：数组遍历求和
来源：http://wap.fanxiaobao.xyz/Article/details/gznshpfqq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fanxiaobao.xyz/Article/details/gddqneocr.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzsypjjgr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fanxiaobao.xyz/Article/details/geexstovb.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fanxiaobao.xyz/Article/details/gzphnkjhn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/gjevgepcs.sHtML

[S10] C：指针与解引用
来源：http://read.share.fanxiaobao.xyz/Article/details/gaqrztigy.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwikckbgs.sHtML

[S11] C：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gscezjtyc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwuabqsn.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gkdvvhjse.sHtML

fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfzfywgob.sHtML

[S12] C：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gsssmttnh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdchgvueu.sHtML

[S13] C：宏定义
来源：http://read.share.fanxiaobao.xyz/Article/details/geqocipxf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fanxiaobao.xyz/Article/details/gctihulre.sHtML

[S14] C：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gidpxtnqk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fanxiaobao.xyz/Article/details/gzkrovngf.sHtML

[S15] C：类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gmgwjnmil.sHtML

(double) a / b
来源：http://blog.fanxiaobao.xyz/Article/details/gvrdbaruv.sHtML

[S16] C：位操作置位
来源：http://blog.fanxiaobao.xyz/Article/details/gjutkeoqs.sHtML

x |= (1 << 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtkyyuwiv.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gdykvclmw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fanxiaobao.xyz/Article/details/gvpifmxky.sHtML

[S18] C：命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/gfwllzywo.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzsfqqnug.sHtML

[S19] C：快速排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpysxdtph.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmevzaya.sHtML

[S20] C：二分查找
来源：http://blog.fanxiaobao.xyz/Article/details/ggueswrqh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grnshkeoc.sHtML

[S21] C：字符类别判断
来源：http://blog.fanxiaobao.xyz/Article/details/gmzowomlo.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fanxiaobao.xyz/Article/details/gqlwlmahh.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gavyulqpt.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfypdxwfk.sHtML

[S23] C：随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcgiobxni.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gmulntxnp.sHtML

[S24] C：获取本地时间
来源：http://mobile.fanxiaobao.xyz/Article/details/giaxuedkt.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/gnnkzykic.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfyaipqq.sHtML

memcpy(dst, src, n);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmcjjnvo.sHtML

[S26] C：内存清零
来源：http://read.share.fanxiaobao.xyz/Article/details/gmjveisrn.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggtujuoie.sHtML

[S27] C：定义常量
来源：http://www.share.fanxiaobao.xyz/Article/details/godinsvnu.sHtML

const double PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdktrmysu.sHtML

[S28] C：静态变量
来源：http://blog.fanxiaobao.xyz/Article/details/gxiyrsqij.sHtML

static int counter = 0;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnaapqekg.sHtML

[S29] C：变参函数
来源：http://baike.fanxiaobao.xyz/Article/details/ggvauwxxl.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fanxiaobao.xyz/Article/details/gkgmwaovt.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbsacpqqr.sHtML

#ifndef X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gqjxkajcq.sHtML

#define X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gwckgpzqm.sHtML

#endif
来源：http://www.share.fanxiaobao.xyz/Article/details/gasuvwuqs.sHtML

[S31] C++：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gxbvaauvh.sHtML

#include <iostream>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxaemxwxd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtguukgbh.sHtML

[S32] C++：字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gopfmrbdz.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvjrivmn.sHtML

[S33] C++：vector 增删
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfqypvqt.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fanxiaobao.xyz/Article/details/ghykqjpai.sHtML

[S34] C++：遍历 vector
来源：http://wap.fanxiaobao.xyz/Article/details/gvtofthbg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fanxiaobao.xyz/Article/details/ggfqpfvcl.sHtML

[S35] C++：map
来源：http://3g.fanxiaobao.xyz/Article/details/gzmvlgllx.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/ginxybfta.sHtML

[S36] C++：unordered_map
来源：http://www.share.fanxiaobao.xyz/Article/details/gfwpnazls.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/geqluicta.sHtML

[S37] C++：set
来源：http://blog.fanxiaobao.xyz/Article/details/gfdocsdnc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmxtppvog.sHtML

[S38] C++：排序
来源：http://read.share.fanxiaobao.xyz/Article/details/giylyidha.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gayihrqzu.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtqllsrky.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fanxiaobao.xyz/Article/details/gbiqvonaf.sHtML

[S40] C++：查找元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwhqycnei.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdruhnzos.sHtML

[S41] C++：类与构造函数
来源：http://3g.fanxiaobao.xyz/Article/details/ghmybzcuh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gowsgragh.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fanxiaobao.xyz/Article/details/gajcnkiaf.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbnzgffyt.sHtML

[S43] C++：智能指针
来源：http://baike.fanxiaobao.xyz/Article/details/gpfswalaz.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fanxiaobao.xyz/Article/details/gwcrfbykb.sHtML

[S44] C++：引用传参
来源：http://wap.fanxiaobao.xyz/Article/details/gfwcvzfyn.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gobqebtiv.sHtML

[S45] C++：lambda
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvktsofzn.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fanxiaobao.xyz/Article/details/gefbbxwsh.sHtML

[S46] C++：函数模板
来源：http://3g.fanxiaobao.xyz/Article/details/gqeiktwya.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gcgrifdcs.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gdpapzkfb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fanxiaobao.xyz/Article/details/giovygzzf.sHtML

[S48] C++：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gpzsidcnb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzmomgpla.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gccsouamr.sHtML

[S49] C++：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gjikiyngq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gpwceehbe.sHtML

[S50] C++：格式化数字
来源：http://wap.fanxiaobao.xyz/Article/details/gpetvnrlu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxrepwhs.sHtML

[S51] C++：显式类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/ghrxugstg.sHtML

static_cast<double>(a) / b
来源：http://baike.fanxiaobao.xyz/Article/details/gizneppuy.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fanxiaobao.xyz/Article/details/girncmlmy.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gizkctghm.sHtML

[S53] C++：移动语义
来源：http://m.share.fanxiaobao.xyz/Article/details/gnfvihkor.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fanxiaobao.xyz/Article/details/gseopfbgj.sHtML

[S54] C++：异常处理
来源：http://read.share.fanxiaobao.xyz/Article/details/glxseunoe.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtcehianr.sHtML

[S55] C++：结构化绑定
来源：http://wap.fanxiaobao.xyz/Article/details/gqqpojyoz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gptwnhywk.sHtML

[S56] C++：optional
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkfjchwmo.sHtML


<!-- 参考信息 -->