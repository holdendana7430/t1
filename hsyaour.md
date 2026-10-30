代发 wailian999

[Q82] 字符长度与字节长度
来源：http://www.share.hesvh.cn/Article/details/gunvwczpy.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gjfbfnaag.sHtML

[Q83] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gfwengmet.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gtrocryrp.sHtML

[Q84] 去除首尾空格
来源：http://blog.hesvh.cn/Article/details/gvbyywbec.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gtcglazwp.sHtML

[Q85] 数值取整
来源：http://m.share.hesvh.cn/Article/details/gekvvmnal.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fehbvm.com/Article/details/gkuvwubfk.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.hesvh.cn/Article/details/gntwinppv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.hesvh.cn/Article/details/gowkavvbx.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.zdbjq.cn/Article/details/gyvvqmegq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.zdbjq.cn/Article/details/gozbjttul.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fehbvm.com/Article/details/gvvqkdzkb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fehbvm.com/Article/details/gzarnkgww.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fehbvm.com/Article/details/giicbcvyh.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gbijeeeoj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.zdbjq.cn/Article/details/gxkrtqbok.sHtML

[Q90] 生成序号列
来源：http://blog.fehbvm.com/Article/details/gltpjtygz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fehbvm.com/Article/details/glvdpqvsw.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gniuojbpv.sHtML

R. Bash 专题
来源：http://www.m.share.zdbjq.cn/Article/details/gkshnnafh.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gnngiwpfe.sHtML

[R01] shebang 与严格模式
来源：http://blog.fehbvm.com/Article/details/gvwnthifz.sHtML

#!/usr/bin/env bash
来源：http://read.share.fehbvm.com/Article/details/ghlnhtyjr.sHtML

set -euo pipefail
来源：http://3g.zdbjq.cn/Article/details/gdhzvaupc.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.zdbjq.cn/Article/details/gxukrmpqm.sHtML

name="Tom"; echo "$name"
来源：http://mobile.zdbjq.cn/Article/details/guvkwugal.sHtML

[R03] 只读变量
来源：http://wap.fehbvm.com/Article/details/glhmlusrv.sHtML

readonly PI=3.14
来源：http://baike.fehbvm.com/Article/details/gdsqxdfex.sHtML

[R04] 位置参数
来源：http://www.m.share.fehbvm.com/Article/details/gbaczllij.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fehbvm.com/Article/details/gdymitbtp.sHtML

[R05] 参数默认值
来源：http://www.share.hesvh.cn/Article/details/gwynroiot.sHtML

name="${1:-default}"
来源：http://read.share.zdbjq.cn/Article/details/gmerxkzjx.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fehbvm.com/Article/details/gfhtkjxta.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/giuxkzsjh.sHtML

[R07] if 判断文件
来源：http://blog.zdbjq.cn/Article/details/gzgmspqfo.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.zdbjq.cn/Article/details/grdyvikba.sHtML

[R08] 数值比较
来源：http://mobile.fehbvm.com/Article/details/glaigyris.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.zdbjq.cn/Article/details/gblqlddtq.sHtML

[R09] 字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gbpecuktl.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.hesvh.cn/Article/details/gqflrxmdq.sHtML

[R10] 正则匹配
来源：http://m.share.zdbjq.cn/Article/details/gtrareukj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.hesvh.cn/Article/details/ghwjuufbg.sHtML

[R11] case 多分支
来源：http://m.share.fehbvm.com/Article/details/gxrkxmzms.sHtML

case "$1" in
来源：http://wap.hesvh.cn/Article/details/gdjnzbrjh.sHtML

start) echo "启动" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gbdcvngaa.sHtML

stop)  echo "停止" ;;
来源：http://3g.hesvh.cn/Article/details/gabsbjenp.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fehbvm.com/Article/details/gfzgjsfpm.sHtML

esac
来源：http://blog.zdbjq.cn/Article/details/gtttkllst.sHtML

[R12] for 遍历文件
来源：http://www.blog.zdbjq.cn/Article/details/gqfwjfdfv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fehbvm.com/Article/details/gfhuzdvli.sHtML

[R13] for 计数循环
来源：http://blog.hesvh.cn/Article/details/gnpsednec.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/gafrxugal.sHtML

[R14] C 风格 for
来源：http://wap.hesvh.cn/Article/details/gbfpykgya.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/gommiixab.sHtML

[R15] while 逐行读文件
来源：http://www.share.fehbvm.com/Article/details/geyjrmxyt.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.zdbjq.cn/Article/details/gwifkyluc.sHtML

[R16] until 等待条件
来源：http://m.share.hesvh.cn/Article/details/gycvqwffm.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/gsigrhyjk.sHtML

[R17] 数组定义与取值
来源：http://www.share.fehbvm.com/Article/details/gxzotmbbg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fehbvm.com/Article/details/gzajfshlk.sHtML

[R18] 遍历数组
来源：http://mobile.hesvh.cn/Article/details/gsxtralyf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fehbvm.com/Article/details/gytljucgb.sHtML

[R19] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gijwndypy.sHtML

echo "${#arr[@]}"
来源：http://baike.hesvh.cn/Article/details/gomfzzpjq.sHtML

[R20] 关联数组（字典）
来源：http://baike.hesvh.cn/Article/details/gzjdytzbk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fehbvm.com/Article/details/ghobobtxx.sHtML

[R21] 字符串长度
来源：http://blog.hesvh.cn/Article/details/gjiqkxwwc.sHtML

echo "${#s}"
来源：http://wap.zdbjq.cn/Article/details/geyqaynlf.sHtML

[R22] 截取子串
来源：http://www.share.fehbvm.com/Article/details/gxexrmcnm.sHtML

echo "${s:0:5}"
来源：http://wap.hesvh.cn/Article/details/gkxhzfbwy.sHtML

[R23] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/gvwylvdqh.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.zdbjq.cn/Article/details/geapfdgfn.sHtML

[R24] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/gorbiqpjt.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.hesvh.cn/Article/details/gjpugcvnl.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fehbvm.com/Article/details/gyvceoukn.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.zdbjq.cn/Article/details/gvkkdrmxk.sHtML

[R26] 命令替换
来源：http://read.share.fehbvm.com/Article/details/gjykeubdh.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.hesvh.cn/Article/details/glovlaqtd.sHtML

[R27] 算术展开
来源：http://mobile.hesvh.cn/Article/details/gjqkcbkiz.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fehbvm.com/Article/details/gzpuwobig.sHtML

[R28] 浮点运算
来源：http://wap.fehbvm.com/Article/details/gzsyipnem.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.hesvh.cn/Article/details/gyzmtwyux.sHtML

[R29] 定义函数
来源：http://www.share.fehbvm.com/Article/details/gehdyzhlt.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.hesvh.cn/Article/details/gilleuxfc.sHtML

[R30] 函数返回状态码
来源：http://m.share.hesvh.cn/Article/details/ggxvkcjce.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.hesvh.cn/Article/details/gmtxefcnt.sHtML

[R31] 局部变量
来源：http://read.share.hesvh.cn/Article/details/gfpfrmmdb.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.hesvh.cn/Article/details/gophfqsey.sHtML

[R32] 参数个数校验
来源：http://3g.fehbvm.com/Article/details/glxdacmiv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fehbvm.com/Article/details/glnqgerpm.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.zdbjq.cn/Article/details/gikzupvbl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fehbvm.com/Article/details/gggoyffsg.sHtML

[R34] 退出时清理
来源：http://read.share.fehbvm.com/Article/details/ghrfpnbfj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/gociyltog.sHtML

[R35] 后台执行并等待
来源：http://mobile.zdbjq.cn/Article/details/gsmagnocd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fehbvm.com/Article/details/gjlwfsijv.sHtML

[R36] 并发执行多个任务
来源：http://wap.zdbjq.cn/Article/details/gnuguisue.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.zdbjq.cn/Article/details/gmhwnspng.sHtML

[R37] 把输出赋给变量
来源：http://read.share.hesvh.cn/Article/details/gxfygmbvu.sHtML

files=$(ls -1)
来源：http://baike.zdbjq.cn/Article/details/gkoqrfrcr.sHtML

[R38] 管道串联
来源：http://blog.hesvh.cn/Article/details/gwpvzhrxx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fehbvm.com/Article/details/gruffywyf.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.hesvh.cn/Article/details/gvflggmrv.sHtML

cmd > out.log 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gytqxpedu.sHtML

[R40] 追加写日志
来源：http://m.share.hesvh.cn/Article/details/gwxdjogfp.sHtML

echo "log" >> out.log
来源：http://m.share.zdbjq.cn/Article/details/gotabbbdb.sHtML

[R41] 丢弃输出
来源：http://www.m.share.zdbjq.cn/Article/details/gscpleqor.sHtML

cmd >/dev/null 2>&1
来源：http://blog.zdbjq.cn/Article/details/gbhlddycy.sHtML

[R42] 输入重定向
来源：http://wap.zdbjq.cn/Article/details/gatisfgsp.sHtML

wc -l < a.txt
来源：http://blog.fehbvm.com/Article/details/gygtkykkg.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.zdbjq.cn/Article/details/ghbseugku.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.hesvh.cn/Article/details/gdgjlfgjr.sHtML

[R44] 按修改时间查找
来源：http://blog.zdbjq.cn/Article/details/gmhtgpacc.sHtML

find . -mtime -7 -type f
来源：http://blog.fehbvm.com/Article/details/gvxmckctk.sHtML

[R45] 批量删除
来源：http://blog.hesvh.cn/Article/details/gmskjmjld.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fehbvm.com/Article/details/gkkxjnyqj.sHtML

[R46] 递归替换文件内容
来源：http://m.share.zdbjq.cn/Article/details/gmocaazts.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fehbvm.com/Article/details/ghpylmrua.sHtML

[R47] sed 单行替换
来源：http://m.share.hesvh.cn/Article/details/gnchrmcfw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.hesvh.cn/Article/details/gubaiinaf.sHtML

[R48] awk 取指定列
来源：http://m.share.fehbvm.com/Article/details/gzzyfwvlc.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gcitdbcik.sHtML

[R49] awk 带条件
来源：http://mobile.zdbjq.cn/Article/details/gjrvmrxwq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.hesvh.cn/Article/details/gdipzzimo.sHtML

[R50] awk 求和
来源：http://read.share.fehbvm.com/Article/details/gcbplqwac.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.hesvh.cn/Article/details/gkvabkosk.sHtML

[R51] 排序去重取前几
来源：http://www.blog.zdbjq.cn/Article/details/gruimkfyb.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.zdbjq.cn/Article/details/gmqtuzndq.sHtML

[R52] 统计行数
来源：http://mobile.hesvh.cn/Article/details/gjgkmskvc.sHtML

wc -l a.txt
来源：http://blog.zdbjq.cn/Article/details/glvrqberx.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.hesvh.cn/Article/details/gsajyujwu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fehbvm.com/Article/details/galohynqu.sHtML

[R54] 比较两个文件
来源：http://www.share.fehbvm.com/Article/details/ghqkgclac.sHtML

diff a.txt b.txt
来源：http://www.blog.hesvh.cn/Article/details/ggpglweug.sHtML

[R55] 压缩与解压
来源：http://www.share.fehbvm.com/Article/details/gkvrzgfwh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.hesvh.cn/Article/details/ganmxizqo.sHtML

[R56] 远程拷贝
来源：http://blog.fehbvm.com/Article/details/gbyntprxc.sHtML

scp file user@host:/path/
来源：http://read.share.fehbvm.com/Article/details/gpodroilo.sHtML

[R57] 远程执行命令
来源：http://wap.fehbvm.com/Article/details/gqzwqbtmv.sHtML

ssh user@host 'uptime'
来源：http://baike.hesvh.cn/Article/details/gyxmyvbzl.sHtML

[R58] 下载文件
来源：http://blog.zdbjq.cn/Article/details/gayzgvraq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fehbvm.com/Article/details/giumjsqax.sHtML

[R59] 发 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/gsylnocba.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.hesvh.cn/Article/details/gklhzpxbj.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.hesvh.cn/Article/details/gyhpwbnkx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.zdbjq.cn/Article/details/gbiqquqwe.sHtML

[R61] 磁盘占用
来源：http://3g.zdbjq.cn/Article/details/gswsbkenb.sHtML

df -h;  du -sh *
来源：http://wap.zdbjq.cn/Article/details/gbevoxhpt.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.hesvh.cn/Article/details/gzhyhjezy.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fehbvm.com/Article/details/gcckinfhe.sHtML

[R63] 内存与进程
来源：http://mobile.zdbjq.cn/Article/details/gejehhxui.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.zdbjq.cn/Article/details/gntukvqwh.sHtML

[R64] 结束进程
来源：http://3g.fehbvm.com/Article/details/grrkcctaw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.hesvh.cn/Article/details/gbvxpxsge.sHtML

[R65] 查看端口占用
来源：http://wap.zdbjq.cn/Article/details/getmshoos.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.zdbjq.cn/Article/details/gkootyreu.sHtML

[R66] 定时任务
来源：http://read.share.hesvh.cn/Article/details/gwtxqnupj.sHtML

crontab -e;  crontab -l
来源：http://blog.hesvh.cn/Article/details/gqcgytodk.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fehbvm.com/Article/details/gxbagsrdd.sHtML

openssl rand -hex 16
来源：http://www.share.fehbvm.com/Article/details/gcbxtbtru.sHtML

[R68] 计算文件校验值
来源：http://wap.hesvh.cn/Article/details/gvgxcdexr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.hesvh.cn/Article/details/gxjiwdlxu.sHtML

[R69] 生成随机密码
来源：http://www.blog.zdbjq.cn/Article/details/gvxghreww.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fehbvm.com/Article/details/gxiflynee.sHtML

[R70] 时间戳与互转
来源：http://www.blog.hesvh.cn/Article/details/gsiarnbnl.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.zdbjq.cn/Article/details/gsdzahszb.sHtML

[R71] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/ggsddnapx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.zdbjq.cn/Article/details/gayhcnndz.sHtML

[R72] 等待端口就绪
来源：http://www.blog.hesvh.cn/Article/details/gnmejnzeo.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/ghbdyrkdx.sHtML

[R73] 分割大日志
来源：http://baike.hesvh.cn/Article/details/gvbivexms.sHtML

split -l 1000 big.log part_
来源：http://baike.fehbvm.com/Article/details/ghpezddut.sHtML

[R74] 批量重命名
来源：http://3g.hesvh.cn/Article/details/gfxzlntko.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.hesvh.cn/Article/details/gbdfyzldk.sHtML

[R75] 导出环境变量
来源：http://3g.fehbvm.com/Article/details/gpirxxukw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.zdbjq.cn/Article/details/gwmxoutkf.sHtML

[R76] 使用临时文件
来源：http://m.share.fehbvm.com/Article/details/gupjswclo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/goxotrlrn.sHtML

[R77] 读取用户输入
来源：http://wap.hesvh.cn/Article/details/gojdoxijk.sHtML

read -rp "请输入: " ans
来源：http://wap.fehbvm.com/Article/details/gopyohctq.sHtML

[R78] 交互式菜单
来源：http://read.share.hesvh.cn/Article/details/gxzrqnwrd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.hesvh.cn/Article/details/ggshotxkg.sHtML

[R79] 解析命令行选项
来源：http://read.share.fehbvm.com/Article/details/gwbgrwoks.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fehbvm.com/Article/details/gsmddlrjj.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fehbvm.com/Article/details/gpybyrpwi.sHtML

time ./run.sh
来源：http://baike.zdbjq.cn/Article/details/ggdoxymyd.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gohxehpzq.sHtML

S. C / C++ 专题
来源：http://www.m.share.zdbjq.cn/Article/details/gpahrwccv.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gwpnsonyc.sHtML

[S01] C：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gtqxteplc.sHtML

#include <stdio.h>
来源：http://read.share.zdbjq.cn/Article/details/gtfqbhgjo.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.hesvh.cn/Article/details/gbjzbljis.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fehbvm.com/Article/details/grungpyxf.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fehbvm.com/Article/details/gswyloigw.sHtML

[S03] C：读入整数
来源：http://m.share.fehbvm.com/Article/details/ggrycgjdj.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fehbvm.com/Article/details/geexqzlth.sHtML

[S04] C：字符串复制
来源：http://read.share.hesvh.cn/Article/details/gqtwdjilm.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.hesvh.cn/Article/details/gkvtvcqzq.sHtML

[S05] C：字符串长度
来源：http://blog.fehbvm.com/Article/details/gtvzfwjha.sHtML

strlen(s)
来源：http://www.blog.hesvh.cn/Article/details/gbanvdnmy.sHtML

[S06] C：字符串比较
来源：http://www.share.hesvh.cn/Article/details/gynhxxupz.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.hesvh.cn/Article/details/gazysxohw.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.hesvh.cn/Article/details/glcczmhqa.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fehbvm.com/Article/details/gjcwuvkqo.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fehbvm.com/Article/details/gfctppqdn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fehbvm.com/Article/details/gonjjvril.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.hesvh.cn/Article/details/guogsetjh.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.hesvh.cn/Article/details/gydskbhmh.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.hesvh.cn/Article/details/gxnibfmmm.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.hesvh.cn/Article/details/gsnsimvfe.sHtML

[S11] C：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/govsavplz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.zdbjq.cn/Article/details/gbbhskkjj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.zdbjq.cn/Article/details/gfprgblzt.sHtML

fclose(f);
来源：http://wap.hesvh.cn/Article/details/gwzvkxrvb.sHtML

[S12] C：写文件
来源：http://mobile.zdbjq.cn/Article/details/gymmrjcuv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/gwwdmhlnr.sHtML

[S13] C：宏定义
来源：http://3g.zdbjq.cn/Article/details/ghezfeeda.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fehbvm.com/Article/details/gbydlxmai.sHtML

[S14] C：枚举
来源：http://www.blog.fehbvm.com/Article/details/gaakideut.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.zdbjq.cn/Article/details/gcfsdjjoj.sHtML

[S15] C：类型转换
来源：http://www.share.hesvh.cn/Article/details/gtsiknbgd.sHtML

(double) a / b
来源：http://www.share.fehbvm.com/Article/details/gqxfyuwid.sHtML

[S16] C：位操作置位
来源：http://www.share.fehbvm.com/Article/details/gsfwryltx.sHtML

x |= (1 << 3);
来源：http://blog.zdbjq.cn/Article/details/gvpkzzqhk.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gevasoopw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fehbvm.com/Article/details/gjktafjjw.sHtML

[S18] C：命令行参数
来源：http://m.share.zdbjq.cn/Article/details/gpdnopmad.sHtML

int main(int argc, char **argv)
来源：http://mobile.fehbvm.com/Article/details/guuvgblyg.sHtML

[S19] C：快速排序
来源：http://3g.fehbvm.com/Article/details/ggoneaiav.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gmqvwbkgg.sHtML

[S20] C：二分查找
来源：http://blog.hesvh.cn/Article/details/gaetdspsb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gfxutdmar.sHtML

[S21] C：字符类别判断
来源：http://m.share.hesvh.cn/Article/details/gewbuqovm.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.hesvh.cn/Article/details/glctehllc.sHtML

[S22] C：字符串转数字
来源：http://read.share.fehbvm.com/Article/details/gnhsghofq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.hesvh.cn/Article/details/gxtncttsy.sHtML

[S23] C：随机数
来源：http://mobile.fehbvm.com/Article/details/gkuoeqbnp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fehbvm.com/Article/details/ghhoujuok.sHtML

[S24] C：获取本地时间
来源：http://www.blog.zdbjq.cn/Article/details/gzyrvepoq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fehbvm.com/Article/details/gglprnigy.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gvcapwmyx.sHtML

memcpy(dst, src, n);
来源：http://mobile.hesvh.cn/Article/details/gveuzgsfr.sHtML

[S26] C：内存清零
来源：http://wap.fehbvm.com/Article/details/gujpjamom.sHtML

memset(a, 0, sizeof a);
来源：http://blog.zdbjq.cn/Article/details/gabwhpelp.sHtML

[S27] C：定义常量
来源：http://3g.fehbvm.com/Article/details/goerohcmj.sHtML

const double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/graojcrwu.sHtML

[S28] C：静态变量
来源：http://mobile.zdbjq.cn/Article/details/gbuagdfmm.sHtML

static int counter = 0;
来源：http://wap.zdbjq.cn/Article/details/gagdpxfbt.sHtML

[S29] C：变参函数
来源：http://www.share.fehbvm.com/Article/details/goxtmezmi.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fehbvm.com/Article/details/ggqvjodot.sHtML

[S30] C：头文件保护
来源：http://read.share.hesvh.cn/Article/details/gdgusjgge.sHtML

#ifndef X_H
来源：http://wap.hesvh.cn/Article/details/gsgnnkwwc.sHtML

#define X_H
来源：http://www.m.share.hesvh.cn/Article/details/gccdhdpqm.sHtML

#endif
来源：http://www.blog.zdbjq.cn/Article/details/gzxjzgkry.sHtML

[S31] C++：Hello World
来源：http://www.blog.hesvh.cn/Article/details/giigdgzmq.sHtML

#include <iostream>
来源：http://wap.zdbjq.cn/Article/details/ggxlpxfuj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.hesvh.cn/Article/details/gnuflegsq.sHtML

[S32] C++：字符串
来源：http://blog.hesvh.cn/Article/details/gbpwwenst.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.zdbjq.cn/Article/details/gwuktzsbi.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.hesvh.cn/Article/details/gqjgbxhgl.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gwjpkdcbu.sHtML

[S34] C++：遍历 vector
来源：http://mobile.zdbjq.cn/Article/details/guzelmpem.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.zdbjq.cn/Article/details/gbgqlhlii.sHtML

[S35] C++：map
来源：http://www.m.share.fehbvm.com/Article/details/grvbduudx.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gvablbuss.sHtML

[S36] C++：unordered_map
来源：http://www.share.zdbjq.cn/Article/details/gqbxhqoin.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gzmhvxeso.sHtML

[S37] C++：set
来源：http://mobile.hesvh.cn/Article/details/garjlhuyr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.zdbjq.cn/Article/details/gilrogkxk.sHtML

[S38] C++：排序
来源：http://www.blog.zdbjq.cn/Article/details/gxyyumlvj.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.hesvh.cn/Article/details/gdzbxfrnm.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.zdbjq.cn/Article/details/gftvqlwqk.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fehbvm.com/Article/details/geedfdncj.sHtML

[S40] C++：查找元素
来源：http://blog.zdbjq.cn/Article/details/gqjfjgdhe.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fehbvm.com/Article/details/glohnstrp.sHtML

[S41] C++：类与构造函数
来源：http://baike.zdbjq.cn/Article/details/gryrcuqxh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.hesvh.cn/Article/details/gqrjpbzut.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.hesvh.cn/Article/details/gdctzxtxg.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.hesvh.cn/Article/details/gcmnrshyz.sHtML

[S43] C++：智能指针
来源：http://www.m.share.zdbjq.cn/Article/details/gorwsiecf.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.hesvh.cn/Article/details/guthypqca.sHtML

[S44] C++：引用传参
来源：http://www.m.share.hesvh.cn/Article/details/gdvtzgzys.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fehbvm.com/Article/details/gxxcdrouy.sHtML

[S45] C++：lambda
来源：http://3g.zdbjq.cn/Article/details/gnfxtfohk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.zdbjq.cn/Article/details/glyqlrnps.sHtML

[S46] C++：函数模板
来源：http://blog.zdbjq.cn/Article/details/gjfvjcrwb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.zdbjq.cn/Article/details/gdyogvhwx.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.zdbjq.cn/Article/details/gbioujeyh.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.zdbjq.cn/Article/details/gtaikbplp.sHtML

[S48] C++：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gpnyhojth.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.hesvh.cn/Article/details/gmaxcrvwd.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fehbvm.com/Article/details/gtqvrpmqk.sHtML

[S49] C++：写文件
来源：http://baike.fehbvm.com/Article/details/gmwlguvwo.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fehbvm.com/Article/details/gqzdewgfc.sHtML

[S50] C++：格式化数字
来源：http://baike.fehbvm.com/Article/details/gpzurdrpn.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gialjbmnt.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gdvhohyxq.sHtML

static_cast<double>(a) / b
来源：http://blog.zdbjq.cn/Article/details/ghzepgsqs.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fehbvm.com/Article/details/ggzvrsood.sHtML


<!-- 参考信息 -->