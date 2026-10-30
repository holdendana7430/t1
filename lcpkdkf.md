代发 wailian999

[Q86] 读取 JSON 字段
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gygebxyyk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fanxiaobao.xyz/Article/details/gtmqbdqih.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gvmkauhwu.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcaguvssy.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gporhrsqm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fanxiaobao.xyz/Article/details/gymsalxza.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/goztxuxbb.sHtML

[Q89] 判断表是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/guutvteuf.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gttvzdsfj.sHtML

[Q90] 生成序号列
来源：http://read.share.fanxiaobao.xyz/Article/details/gzrnollnp.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqgxffwbt.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gsnhwwbcb.sHtML

R. Bash 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gapuypdlx.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gaddkfadn.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsrpmkksy.sHtML

#!/usr/bin/env bash
来源：http://mobile.fanxiaobao.xyz/Article/details/gstvzkned.sHtML

set -euo pipefail
来源：http://read.share.fanxiaobao.xyz/Article/details/gdabosfnb.sHtML

[R02] 变量赋值与使用
来源：http://baike.fanxiaobao.xyz/Article/details/gifsetrlq.sHtML

name="Tom"; echo "$name"
来源：http://baike.fanxiaobao.xyz/Article/details/ghgpdiowy.sHtML

[R03] 只读变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gptqeaslq.sHtML

readonly PI=3.14
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmkhkjxq.sHtML

[R04] 位置参数
来源：http://3g.fanxiaobao.xyz/Article/details/gqijivxew.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghvlvpkei.sHtML

[R05] 参数默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/gtgyiabvi.sHtML

name="${1:-default}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gukietfba.sHtML

[R06] 判断命令是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/gzqhfrblg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/grbqdlnud.sHtML

[R07] if 判断文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbzzcafs.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/grmgaovix.sHtML

[R08] 数值比较
来源：http://wap.fanxiaobao.xyz/Article/details/gymtmbnmy.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gzjfntyye.sHtML

[R09] 字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gdpqrqrtn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/giuidtyod.sHtML

[R10] 正则匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gzlzhnkyq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/givumqxmg.sHtML

[R11] case 多分支
来源：http://www.share.fanxiaobao.xyz/Article/details/gubyoqcsi.sHtML

case "$1" in
来源：http://m.share.fanxiaobao.xyz/Article/details/goqoasmzk.sHtML

start) echo "启动" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwgteudgl.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpvrdrkaa.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gvzqmunit.sHtML

esac
来源：http://wap.fanxiaobao.xyz/Article/details/gqftqlicj.sHtML

[R12] for 遍历文件
来源：http://blog.fanxiaobao.xyz/Article/details/gfuuygaqi.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/golbanhcf.sHtML

[R13] for 计数循环
来源：http://wap.fanxiaobao.xyz/Article/details/gqcsyzmjw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/ggtbqgxdq.sHtML

[R14] C 风格 for
来源：http://baike.fanxiaobao.xyz/Article/details/gslknzucc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gqwncloxo.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gancnwabg.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghlqbykhp.sHtML

[R16] until 等待条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gozymsguy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gcmrybtsk.sHtML

[R17] 数组定义与取值
来源：http://3g.fanxiaobao.xyz/Article/details/gzyfqhgcb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjmdevodl.sHtML

[R18] 遍历数组
来源：http://3g.fanxiaobao.xyz/Article/details/gxpgnmkli.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gexfojvey.sHtML

[R19] 数组长度
来源：http://blog.fanxiaobao.xyz/Article/details/gazagulit.sHtML

echo "${#arr[@]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gvixfolrt.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbmcywgj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqyjdakei.sHtML

[R21] 字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gteniuwsy.sHtML

echo "${#s}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtzjtyagv.sHtML

[R22] 截取子串
来源：http://www.share.fanxiaobao.xyz/Article/details/grrxhbkuj.sHtML

echo "${s:0:5}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gpubragvj.sHtML

[R23] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gjgyztgka.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gvwpyutvi.sHtML

[R24] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gbprqlujh.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fanxiaobao.xyz/Article/details/gtazxtifi.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fanxiaobao.xyz/Article/details/gxjlkzfuq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gvrykezkm.sHtML

[R26] 命令替换
来源：http://blog.fanxiaobao.xyz/Article/details/gopccfdqv.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fanxiaobao.xyz/Article/details/gorhgjgln.sHtML

[R27] 算术展开
来源：http://read.share.fanxiaobao.xyz/Article/details/gydyejjbx.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gignvfdol.sHtML

[R28] 浮点运算
来源：http://read.share.fanxiaobao.xyz/Article/details/gcidqyhff.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fanxiaobao.xyz/Article/details/gaqnjwtyc.sHtML

[R29] 定义函数
来源：http://3g.fanxiaobao.xyz/Article/details/gnkfesisn.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkaogmikh.sHtML

[R30] 函数返回状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gcujaufmm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fanxiaobao.xyz/Article/details/gyeanpeew.sHtML

[R31] 局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/gdslpmino.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fanxiaobao.xyz/Article/details/ggspndbil.sHtML

[R32] 参数个数校验
来源：http://mobile.fanxiaobao.xyz/Article/details/gwdgpvksd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gkdutqbjh.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpxxbyjhs.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcrsnxlcb.sHtML

[R34] 退出时清理
来源：http://3g.fanxiaobao.xyz/Article/details/guamvuwac.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvusumewq.sHtML

[R35] 后台执行并等待
来源：http://www.share.fanxiaobao.xyz/Article/details/gfzijszww.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fanxiaobao.xyz/Article/details/gwjeyhple.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fanxiaobao.xyz/Article/details/ggrwnfshf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fanxiaobao.xyz/Article/details/gwfnjkewy.sHtML

[R37] 把输出赋给变量
来源：http://wap.fanxiaobao.xyz/Article/details/gtqizrsce.sHtML

files=$(ls -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjlnnxaf.sHtML

[R38] 管道串联
来源：http://wap.fanxiaobao.xyz/Article/details/gpyhmryjq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gzjvzhqun.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fanxiaobao.xyz/Article/details/gejmarleu.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gtkvsqdfo.sHtML

[R40] 追加写日志
来源：http://blog.fanxiaobao.xyz/Article/details/gnwddkiyg.sHtML

echo "log" >> out.log
来源：http://3g.fanxiaobao.xyz/Article/details/gljtjtlkj.sHtML

[R41] 丢弃输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvcrqgada.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebrpzoes.sHtML

[R42] 输入重定向
来源：http://mobile.fanxiaobao.xyz/Article/details/gxgcdlznd.sHtML

wc -l < a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/ggvnbevig.sHtML

[R43] 按名字查找文件
来源：http://wap.fanxiaobao.xyz/Article/details/gojrmbgus.sHtML

find . -name "*.log" -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gctzjyynb.sHtML

[R44] 按修改时间查找
来源：http://blog.fanxiaobao.xyz/Article/details/gwureagac.sHtML

find . -mtime -7 -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/ggeqndqbi.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/grpajgpow.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fanxiaobao.xyz/Article/details/gpmttflxw.sHtML

[R46] 递归替换文件内容
来源：http://wap.fanxiaobao.xyz/Article/details/gnnslntmc.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fanxiaobao.xyz/Article/details/gizhjhmnl.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gdppfiamp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gshztcxhm.sHtML

[R48] awk 取指定列
来源：http://www.share.fanxiaobao.xyz/Article/details/giexfocqw.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gfyhcyazi.sHtML

[R49] awk 带条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gzhdoaqkn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fanxiaobao.xyz/Article/details/gsnxbiigw.sHtML

[R50] awk 求和
来源：http://3g.fanxiaobao.xyz/Article/details/gmziwcrbj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gmugqslkk.sHtML

[R51] 排序去重取前几
来源：http://baike.fanxiaobao.xyz/Article/details/gsgjqnexu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhlcczqn.sHtML

[R52] 统计行数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/golaacbve.sHtML

wc -l a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gognbydsp.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fanxiaobao.xyz/Article/details/gzjaipynb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fanxiaobao.xyz/Article/details/gejgtekxg.sHtML

[R54] 比较两个文件
来源：http://3g.fanxiaobao.xyz/Article/details/gmqieflvy.sHtML

diff a.txt b.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/ghcvqvuao.sHtML

[R55] 压缩与解压
来源：http://blog.fanxiaobao.xyz/Article/details/gpxjjkskz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fanxiaobao.xyz/Article/details/gleuvsgxa.sHtML

[R56] 远程拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmsgnxwma.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/gbgjbvtov.sHtML

[R57] 远程执行命令
来源：http://baike.fanxiaobao.xyz/Article/details/gkeqosdkt.sHtML

ssh user@host 'uptime'
来源：http://www.share.fanxiaobao.xyz/Article/details/geggovlmv.sHtML

[R58] 下载文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqzzcrvvo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/gabdkgpip.sHtML

[R59] 发 POST JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gjaewagei.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fanxiaobao.xyz/Article/details/gwgpjgxyi.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmvtnffdn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fanxiaobao.xyz/Article/details/gqhtycvcd.sHtML

[R61] 磁盘占用
来源：http://blog.fanxiaobao.xyz/Article/details/ghvysebjc.sHtML

df -h;  du -sh *
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdikhsme.sHtML

[R62] 找最占空间的文件
来源：http://blog.fanxiaobao.xyz/Article/details/grouawkyk.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fanxiaobao.xyz/Article/details/gdcvwykzi.sHtML

[R63] 内存与进程
来源：http://wap.fanxiaobao.xyz/Article/details/gbrelngez.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fanxiaobao.xyz/Article/details/geoqumezl.sHtML

[R64] 结束进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gsicdnxnd.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fanxiaobao.xyz/Article/details/gejslfvwj.sHtML

[R65] 查看端口占用
来源：http://wap.fanxiaobao.xyz/Article/details/gipguizls.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fanxiaobao.xyz/Article/details/gllapoena.sHtML

[R66] 定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/glbtpapye.sHtML

crontab -e;  crontab -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gjsfellcg.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fanxiaobao.xyz/Article/details/gpfrznvpd.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/guswupoik.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gubiqvjqr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gluodcqeg.sHtML

[R69] 生成随机密码
来源：http://www.share.fanxiaobao.xyz/Article/details/gchmsajpa.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fanxiaobao.xyz/Article/details/gzvutrefh.sHtML

[R70] 时间戳与互转
来源：http://blog.fanxiaobao.xyz/Article/details/gwvgdozkb.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fanxiaobao.xyz/Article/details/gvvdglmrk.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/ggqxcwrmg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwyfjdwm.sHtML

[R72] 等待端口就绪
来源：http://wap.fanxiaobao.xyz/Article/details/gnvrllzdf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gwuvpejxw.sHtML

[R73] 分割大日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gincsuqhf.sHtML

split -l 1000 big.log part_
来源：http://mobile.fanxiaobao.xyz/Article/details/gjgffpysk.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/gowtxanis.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gerhjkwnp.sHtML

[R75] 导出环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbdrirqr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxgybaqtr.sHtML

[R76] 使用临时文件
来源：http://mobile.fanxiaobao.xyz/Article/details/glnxavxkb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gnrcdibqk.sHtML

[R77] 读取用户输入
来源：http://www.share.fanxiaobao.xyz/Article/details/gsugsekri.sHtML

read -rp "请输入: " ans
来源：http://mobile.fanxiaobao.xyz/Article/details/gbhkutlwz.sHtML

[R78] 交互式菜单
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbjivkobg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gqskzgxdi.sHtML

[R79] 解析命令行选项
来源：http://mobile.fanxiaobao.xyz/Article/details/ggdlwzlxi.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gzninhuzh.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fanxiaobao.xyz/Article/details/gzfnfbmsv.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/gshgzqtnu.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxuhfvyii.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gpwezmapg.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gmhlpnyeh.sHtML

[S01] C：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gabrufjki.sHtML

#include <stdio.h>
来源：http://mobile.fanxiaobao.xyz/Article/details/gpgqkpwjy.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fanxiaobao.xyz/Article/details/gegibnvjz.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gljljzdqv.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fanxiaobao.xyz/Article/details/gjbaszseu.sHtML

[S03] C：读入整数
来源：http://read.share.fanxiaobao.xyz/Article/details/gtmuoypjs.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwkpqbfny.sHtML

[S04] C：字符串复制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnbyvwbry.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/gwvihxzga.sHtML

[S05] C：字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gytclvptx.sHtML

strlen(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcjorglgm.sHtML

[S06] C：字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/grnyvrdzh.sHtML

strcmp(a, b) == 0
来源：http://baike.fanxiaobao.xyz/Article/details/gymysrpgr.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpevyabdr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggqusrhby.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtrxnclqe.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glopkwyrv.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fanxiaobao.xyz/Article/details/gwtvzjmrt.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fanxiaobao.xyz/Article/details/grnxakdnl.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/gpodhrgao.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fanxiaobao.xyz/Article/details/gvpeknops.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyoqgtbiz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmdmqaety.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzversjki.sHtML

fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/genivlhhs.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/glaykjfix.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gegvrrsux.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gytlgaqqj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fanxiaobao.xyz/Article/details/gbusoflil.sHtML

[S14] C：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gnxsqvntu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxcodpoy.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gqjxfshok.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/gatebgosg.sHtML

[S16] C：位操作置位
来源：http://blog.fanxiaobao.xyz/Article/details/geabluylq.sHtML

x |= (1 << 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gjuyujbxg.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gwbxarnvc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fanxiaobao.xyz/Article/details/gilptjail.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/girptbtou.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtzsypner.sHtML

[S19] C：快速排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmjtafgxb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqrnnsrh.sHtML

[S20] C：二分查找
来源：http://wap.fanxiaobao.xyz/Article/details/gxoefnabu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gvtazqcte.sHtML

[S21] C：字符类别判断
来源：http://mobile.fanxiaobao.xyz/Article/details/grthzzljs.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/glviyeshx.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gnwqtncvt.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fanxiaobao.xyz/Article/details/grbqumdgw.sHtML

[S23] C：随机数
来源：http://read.share.fanxiaobao.xyz/Article/details/gfogqqira.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjurcojky.sHtML

[S24] C：获取本地时间
来源：http://baike.fanxiaobao.xyz/Article/details/gbhgpfwsh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fanxiaobao.xyz/Article/details/gzoseqyme.sHtML

[S25] C：内存拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gdvpgpvds.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsdnqypms.sHtML

[S26] C：内存清零
来源：http://blog.fanxiaobao.xyz/Article/details/giiowpyjs.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fanxiaobao.xyz/Article/details/gaezdwoha.sHtML

[S27] C：定义常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gasybzqdx.sHtML

const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gghidmfsw.sHtML

[S28] C：静态变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnheohlie.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvyeigqbn.sHtML

[S29] C：变参函数
来源：http://3g.fanxiaobao.xyz/Article/details/gwlkmzvlh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grkarxfeg.sHtML

[S30] C：头文件保护
来源：http://baike.fanxiaobao.xyz/Article/details/grvpmeepn.sHtML

#ifndef X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfzwodgmz.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gcdpzndof.sHtML

#endif
来源：http://mobile.fanxiaobao.xyz/Article/details/gvbslmnsa.sHtML

[S31] C++：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/genlyytjw.sHtML

#include <iostream>
来源：http://m.share.fanxiaobao.xyz/Article/details/gpkmklupy.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvdnouleg.sHtML

[S32] C++：字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwrayoek.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywxtgfrt.sHtML

[S33] C++：vector 增删
来源：http://wap.fanxiaobao.xyz/Article/details/gquouflbu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwgunoese.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxplmigrz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnajtprau.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/gxamabfmk.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gkuhzptvi.sHtML

[S36] C++：unordered_map
来源：http://mobile.fanxiaobao.xyz/Article/details/gyblbjzpq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gicehokzh.sHtML

[S37] C++：set
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmxhommb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gwzwwncmp.sHtML

[S38] C++：排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gskcbpopn.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gpyemngsv.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gfimicsie.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fanxiaobao.xyz/Article/details/gbdpjuzbx.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqsghgqg.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhnuihiv.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/giobstxwz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gofvivgfx.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fanxiaobao.xyz/Article/details/gzbrvdfdt.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fanxiaobao.xyz/Article/details/gadiaypby.sHtML

[S43] C++：智能指针
来源：http://m.share.fanxiaobao.xyz/Article/details/gfanabamy.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdvmaqnqm.sHtML

[S44] C++：引用传参
来源：http://3g.fanxiaobao.xyz/Article/details/gcuuvabug.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcrseclcl.sHtML

[S45] C++：lambda
来源：http://mobile.fanxiaobao.xyz/Article/details/guvjmawth.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwdzfkcky.sHtML

[S46] C++：函数模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gvsgeunkk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gknaxcert.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gvwjlwnfc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fanxiaobao.xyz/Article/details/gfandxryc.sHtML

[S48] C++：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gylgozuid.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fanxiaobao.xyz/Article/details/gumdqybkp.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghttdeyab.sHtML

[S49] C++：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gorgijdwx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/gekkzowhy.sHtML

[S50] C++：格式化数字
来源：http://blog.fanxiaobao.xyz/Article/details/gzvbfaxmc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkiegvfzx.sHtML

[S51] C++：显式类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gomgeleat.sHtML

static_cast<double>(a) / b
来源：http://baike.fanxiaobao.xyz/Article/details/gvbwtgibs.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fanxiaobao.xyz/Article/details/gkudytfzf.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gifcttmzs.sHtML

[S53] C++：移动语义
来源：http://wap.fanxiaobao.xyz/Article/details/gogtrnfsp.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxmxgxyly.sHtML

[S54] C++：异常处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gmtdrbfqh.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fanxiaobao.xyz/Article/details/guqszqyax.sHtML

[S55] C++：结构化绑定
来源：http://wap.fanxiaobao.xyz/Article/details/ggykyhwwc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkgwzevte.sHtML

[S56] C++：optional
来源：http://wap.fanxiaobao.xyz/Article/details/gezddskhh.sHtML


<!-- 参考信息 -->