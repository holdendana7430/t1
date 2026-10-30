代发 wailian999

[Q86] 读取 JSON 字段
来源：http://mobile.fanxiaobao.xyz/Article/details/gmzkvtkmn.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fanxiaobao.xyz/Article/details/gjgrgycbo.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkefpxlah.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fanxiaobao.xyz/Article/details/gzrxwfhhe.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fanxiaobao.xyz/Article/details/glnleceti.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fanxiaobao.xyz/Article/details/gatlnvohm.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbttepmwk.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtkpjcmyo.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/gzijktbkb.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqesgqhyo.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjbbqxtng.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gerfooqgu.sHtML

R. Bash 专题
来源：http://3g.fanxiaobao.xyz/Article/details/glduzmmul.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/grldfymfe.sHtML

[R01] shebang 与严格模式
来源：http://blog.fanxiaobao.xyz/Article/details/gnpbwwdqe.sHtML

#!/usr/bin/env bash
来源：http://baike.fanxiaobao.xyz/Article/details/gvioavzro.sHtML

set -euo pipefail
来源：http://read.share.fanxiaobao.xyz/Article/details/gmxxtcikj.sHtML

[R02] 变量赋值与使用
来源：http://wap.fanxiaobao.xyz/Article/details/glvmvkhal.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbdctibpe.sHtML

[R03] 只读变量
来源：http://baike.fanxiaobao.xyz/Article/details/gesztsyea.sHtML

readonly PI=3.14
来源：http://www.share.fanxiaobao.xyz/Article/details/gvklgdbfd.sHtML

[R04] 位置参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gykvudhcm.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fanxiaobao.xyz/Article/details/gfsojqsaj.sHtML

[R05] 参数默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvqbnkbe.sHtML

name="${1:-default}"
来源：http://read.share.fanxiaobao.xyz/Article/details/ghagrmhyv.sHtML

[R06] 判断命令是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/gjhueviaw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gelcexlrm.sHtML

[R07] if 判断文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gilhlugtk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gmvrxehvj.sHtML

[R08] 数值比较
来源：http://3g.fanxiaobao.xyz/Article/details/guhskxgwm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/ggkfdegrb.sHtML

[R09] 字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gqzzjtdlb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmtnrdaq.sHtML

[R10] 正则匹配
来源：http://blog.fanxiaobao.xyz/Article/details/ggnfyjpzb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gkboumoak.sHtML

[R11] case 多分支
来源：http://3g.fanxiaobao.xyz/Article/details/gdpobzqro.sHtML

case "$1" in
来源：http://www.share.fanxiaobao.xyz/Article/details/gucptzntj.sHtML

start) echo "启动" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gehagzowg.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnzysjqsj.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/glaamtttw.sHtML

esac
来源：http://3g.fanxiaobao.xyz/Article/details/gjxwnihoi.sHtML

[R12] for 遍历文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gtutpdvsf.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gklwnxkoe.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/glqbdlkpr.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gldsbwnbz.sHtML

[R14] C 风格 for
来源：http://read.share.fanxiaobao.xyz/Article/details/gqgteuwcg.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxifjdpp.sHtML

[R15] while 逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/guagtmdde.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gaofmvzff.sHtML

[R16] until 等待条件
来源：http://wap.fanxiaobao.xyz/Article/details/gsdgefxjp.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/ggsxcrsgw.sHtML

[R17] 数组定义与取值
来源：http://wap.fanxiaobao.xyz/Article/details/gtibyfenz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gayxtvnvk.sHtML

[R18] 遍历数组
来源：http://baike.fanxiaobao.xyz/Article/details/gyjxiyten.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gldyyhqri.sHtML

[R19] 数组长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/goynsvkwc.sHtML

echo "${#arr[@]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gtetjbzcq.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fanxiaobao.xyz/Article/details/gvajxfnmp.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gylbyivbn.sHtML

[R21] 字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gndgprwwu.sHtML

echo "${#s}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gylqbrjfw.sHtML

[R22] 截取子串
来源：http://baike.fanxiaobao.xyz/Article/details/grfwgnjer.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggpiakcjq.sHtML

[R23] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/guieudeme.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gqazipyzg.sHtML

[R24] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/geepqahgc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fanxiaobao.xyz/Article/details/gybthfjtg.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fanxiaobao.xyz/Article/details/gjmljlpil.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fanxiaobao.xyz/Article/details/gblyqegza.sHtML

[R26] 命令替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gqswgymfz.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fanxiaobao.xyz/Article/details/gjjfvdaky.sHtML

[R27] 算术展开
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtnqjawd.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjaxbgsxl.sHtML

[R28] 浮点运算
来源：http://baike.fanxiaobao.xyz/Article/details/gprizcaro.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwzklzze.sHtML

[R29] 定义函数
来源：http://m.share.fanxiaobao.xyz/Article/details/glchtyxcq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fanxiaobao.xyz/Article/details/gijhmahdm.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/glejaxefg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fanxiaobao.xyz/Article/details/gtvrjbygq.sHtML

[R31] 局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gqcxofltw.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fanxiaobao.xyz/Article/details/glwrrvskd.sHtML

[R32] 参数个数校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gyuyablkl.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbvdiadwz.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/gnrtovrcg.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fanxiaobao.xyz/Article/details/guhfvbbmp.sHtML

[R34] 退出时清理
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghgjfkpxu.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gyzhlcluc.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjvwfzih.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fanxiaobao.xyz/Article/details/gapfogarb.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govxruotv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fanxiaobao.xyz/Article/details/gkheoqxmz.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gfledcvgg.sHtML

files=$(ls -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvnwsikjz.sHtML

[R38] 管道串联
来源：http://mobile.fanxiaobao.xyz/Article/details/gqqftbbzj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fanxiaobao.xyz/Article/details/gcttcxjlp.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fanxiaobao.xyz/Article/details/glncbdlwr.sHtML

cmd > out.log 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gyloixjvw.sHtML

[R40] 追加写日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gdjcistuw.sHtML

echo "log" >> out.log
来源：http://3g.fanxiaobao.xyz/Article/details/gqontmmir.sHtML

[R41] 丢弃输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfjqgvpt.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gsewoldlz.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbjzidlv.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghkjdesau.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejumigcy.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gnqbjhsoz.sHtML

[R44] 按修改时间查找
来源：http://3g.fanxiaobao.xyz/Article/details/glywxlork.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/ggbwucwho.sHtML

[R45] 批量删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gecrgyfrf.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fanxiaobao.xyz/Article/details/gufnlhxkh.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/gqtjewjsn.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtnrlebyb.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmonmzgps.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmegxerr.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gorrlurre.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gxbquuguh.sHtML

[R49] awk 带条件
来源：http://baike.fanxiaobao.xyz/Article/details/gmarztfqu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fanxiaobao.xyz/Article/details/gtgqzvmzg.sHtML

[R50] awk 求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gpkzarcdp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gmfrzhhox.sHtML

[R51] 排序去重取前几
来源：http://3g.fanxiaobao.xyz/Article/details/gxultbocr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fanxiaobao.xyz/Article/details/gbkjlquwu.sHtML

[R52] 统计行数
来源：http://m.share.fanxiaobao.xyz/Article/details/guonizsit.sHtML

wc -l a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnrpihrvt.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fanxiaobao.xyz/Article/details/gdmyyywus.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fanxiaobao.xyz/Article/details/gmkxsjzul.sHtML

[R54] 比较两个文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gevfpekse.sHtML

diff a.txt b.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gukhcbcko.sHtML

[R55] 压缩与解压
来源：http://blog.fanxiaobao.xyz/Article/details/gvfffqqor.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fanxiaobao.xyz/Article/details/gtpedvusx.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsgemuguo.sHtML

scp file user@host:/path/
来源：http://m.share.fanxiaobao.xyz/Article/details/gxlhikecm.sHtML

[R57] 远程执行命令
来源：http://blog.fanxiaobao.xyz/Article/details/gjgvnxchd.sHtML

ssh user@host 'uptime'
来源：http://blog.fanxiaobao.xyz/Article/details/gddgnxcmg.sHtML

[R58] 下载文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggejjqhip.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fanxiaobao.xyz/Article/details/gdrzjioqb.sHtML

[R59] 发 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gxljviuat.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fanxiaobao.xyz/Article/details/gmssuzeet.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjexoounj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fanxiaobao.xyz/Article/details/gyytybunb.sHtML

[R61] 磁盘占用
来源：http://baike.fanxiaobao.xyz/Article/details/gwpmjaidc.sHtML

df -h;  du -sh *
来源：http://3g.fanxiaobao.xyz/Article/details/gaelqggqr.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fanxiaobao.xyz/Article/details/giqzvlpvb.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grmrmkyxo.sHtML

[R63] 内存与进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/goilyrfcn.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fanxiaobao.xyz/Article/details/gdnleyvaj.sHtML

[R64] 结束进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexexlvdw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsnmenapx.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/glytrerdm.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fanxiaobao.xyz/Article/details/gqdekjjky.sHtML

[R66] 定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxzehyuej.sHtML

crontab -e;  crontab -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gvyzzlray.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fanxiaobao.xyz/Article/details/gggjjqpoh.sHtML

openssl rand -hex 16
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbmsdvtm.sHtML

[R68] 计算文件校验值
来源：http://baike.fanxiaobao.xyz/Article/details/grvlramrx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gfkawfogd.sHtML

[R69] 生成随机密码
来源：http://wap.fanxiaobao.xyz/Article/details/gisyhzbrj.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/gyamcskzq.sHtML

[R70] 时间戳与互转
来源：http://blog.fanxiaobao.xyz/Article/details/ghjduidvg.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbvvjlaq.sHtML

[R71] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gwzkyiqfm.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fanxiaobao.xyz/Article/details/giwqfoorp.sHtML

[R72] 等待端口就绪
来源：http://wap.fanxiaobao.xyz/Article/details/gjmkthxau.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gouhdnplw.sHtML

[R73] 分割大日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gtpsiqneo.sHtML

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/gwsaqkgnk.sHtML

[R74] 批量重命名
来源：http://www.share.fanxiaobao.xyz/Article/details/gmncojkvw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gdoyweayv.sHtML

[R75] 导出环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/grpanvmel.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fanxiaobao.xyz/Article/details/gbwyvuhii.sHtML

[R76] 使用临时文件
来源：http://baike.fanxiaobao.xyz/Article/details/gnmegifjs.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gouajjwyd.sHtML

[R77] 读取用户输入
来源：http://wap.fanxiaobao.xyz/Article/details/gfhrawbns.sHtML

read -rp "请输入: " ans
来源：http://mobile.fanxiaobao.xyz/Article/details/gymxsvlwy.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/gandhgcfx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fanxiaobao.xyz/Article/details/gxiojyfhb.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdtxnefod.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fanxiaobao.xyz/Article/details/gzlkphujw.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fanxiaobao.xyz/Article/details/gkfibftuh.sHtML

time ./run.sh
来源：http://m.share.fanxiaobao.xyz/Article/details/gjijcdtmu.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmplihbd.sHtML

S. C / C++ 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gyafjnili.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gkxbmweuk.sHtML

[S01] C：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/guxkkupot.sHtML

#include <stdio.h>
来源：http://baike.fanxiaobao.xyz/Article/details/glclszmpn.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmlumaytf.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gbglvqnoz.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/gkplszfqi.sHtML

[S03] C：读入整数
来源：http://wap.fanxiaobao.xyz/Article/details/gtvloyhuo.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fanxiaobao.xyz/Article/details/gcnwhbfay.sHtML

[S04] C：字符串复制
来源：http://mobile.fanxiaobao.xyz/Article/details/gcqzplmom.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/gurghuhht.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gldoqjcyg.sHtML

strlen(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaaysdciz.sHtML

[S06] C：字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gfrhvkejz.sHtML

strcmp(a, b) == 0
来源：http://mobile.fanxiaobao.xyz/Article/details/ggelmswym.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/gqeqolarc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmfidvddw.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fanxiaobao.xyz/Article/details/gukymbwwu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glfggvtio.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fanxiaobao.xyz/Article/details/gryziszmd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/gfylngenv.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/gmljxuhwa.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fanxiaobao.xyz/Article/details/gwtskzsxj.sHtML

[S11] C：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/ghrmcrfnp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fanxiaobao.xyz/Article/details/geufthbhp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfzrltzkd.sHtML

fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfocdehcg.sHtML

[S12] C：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gjmziviqo.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gupgtbvto.sHtML

[S13] C：宏定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsymutxwl.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fanxiaobao.xyz/Article/details/gzwewexzv.sHtML

[S14] C：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnwknnrvq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fanxiaobao.xyz/Article/details/gxowykrfc.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gmlmvdvdv.sHtML

(double) a / b
来源：http://wap.fanxiaobao.xyz/Article/details/ggyearbqe.sHtML

[S16] C：位操作置位
来源：http://3g.fanxiaobao.xyz/Article/details/gairozgoe.sHtML

x |= (1 << 3);
来源：http://blog.fanxiaobao.xyz/Article/details/grlsxwubc.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/glnkejlrk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fanxiaobao.xyz/Article/details/gidjkoiby.sHtML

[S18] C：命令行参数
来源：http://baike.fanxiaobao.xyz/Article/details/gvmryfcmw.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glmscnqwx.sHtML

[S19] C：快速排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzfqdbamh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gkzacjhfg.sHtML

[S20] C：二分查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfyrifmvd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/ggxtdzazf.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gxqkjgwho.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fanxiaobao.xyz/Article/details/gzqdchtlo.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gasmpczmj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fanxiaobao.xyz/Article/details/gfzszlwhf.sHtML

[S23] C：随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxijenhxe.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghvrlcnxw.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqolvhuor.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fanxiaobao.xyz/Article/details/gggwebjql.sHtML

[S25] C：内存拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gvyvpqcxk.sHtML

memcpy(dst, src, n);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbqqavjlf.sHtML

[S26] C：内存清零
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnieighaq.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fanxiaobao.xyz/Article/details/gvthyyeve.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/gvijfminb.sHtML

const double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/glubdayrf.sHtML

[S28] C：静态变量
来源：http://blog.fanxiaobao.xyz/Article/details/ggauktfpn.sHtML

static int counter = 0;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzhitkbku.sHtML

[S29] C：变参函数
来源：http://3g.fanxiaobao.xyz/Article/details/guyzuihhf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwygzqgch.sHtML

[S30] C：头文件保护
来源：http://read.share.fanxiaobao.xyz/Article/details/gfdqytnco.sHtML

#ifndef X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gntkctlwq.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqehpgyj.sHtML

#endif
来源：http://3g.fanxiaobao.xyz/Article/details/goippzobh.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzizmvll.sHtML

#include <iostream>
来源：http://read.share.fanxiaobao.xyz/Article/details/gttwnfqwv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gdtjzmapr.sHtML

[S32] C++：字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gljxcoysa.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fanxiaobao.xyz/Article/details/gxdmnotay.sHtML

[S33] C++：vector 增删
来源：http://wap.fanxiaobao.xyz/Article/details/gmnhauais.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/godzqqsba.sHtML

[S34] C++：遍历 vector
来源：http://blog.fanxiaobao.xyz/Article/details/gtylzeakt.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpqatbkmo.sHtML

[S35] C++：map
来源：http://mobile.fanxiaobao.xyz/Article/details/gdodsboln.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdeobfiwp.sHtML

[S36] C++：unordered_map
来源：http://baike.fanxiaobao.xyz/Article/details/ghzimpnmu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtnrjnois.sHtML

[S37] C++：set
来源：http://blog.fanxiaobao.xyz/Article/details/ghdwedyop.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvigemryr.sHtML

[S38] C++：排序
来源：http://3g.fanxiaobao.xyz/Article/details/gwklpoowg.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpnbbxgtt.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gnrdsugks.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fanxiaobao.xyz/Article/details/glmdeoupi.sHtML

[S40] C++：查找元素
来源：http://blog.fanxiaobao.xyz/Article/details/gcfhefakr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gtfdcnrfp.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqsbosuqq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fanxiaobao.xyz/Article/details/gumybmhjj.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gstcwevmo.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/gcuxddmgd.sHtML

[S43] C++：智能指针
来源：http://www.blog.fanxiaobao.xyz/Article/details/gokzzmmpd.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fanxiaobao.xyz/Article/details/gwqobugbv.sHtML

[S44] C++：引用传参
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcckdcaos.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/glnupbwms.sHtML

[S45] C++：lambda
来源：http://blog.fanxiaobao.xyz/Article/details/gfgpxgjai.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fanxiaobao.xyz/Article/details/ghbrmdwst.sHtML

[S46] C++：函数模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gduqqmndp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqeehhjde.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gpzzppnul.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkytbmpij.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gnxxznidc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fanxiaobao.xyz/Article/details/gwegmzank.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/ggljjvswx.sHtML

[S49] C++：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gbfnjtvbo.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gpxkuvwac.sHtML

[S50] C++：格式化数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gwdeurvlq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdyavkuvn.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqrfxaig.sHtML

static_cast<double>(a) / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gskyrhwuh.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fanxiaobao.xyz/Article/details/gttdvfdpb.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gghctxluj.sHtML

[S53] C++：移动语义
来源：http://baike.fanxiaobao.xyz/Article/details/gzwoypext.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fanxiaobao.xyz/Article/details/guylfnyse.sHtML

[S54] C++：异常处理
来源：http://3g.fanxiaobao.xyz/Article/details/glhvlcdzj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcevvszmx.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/gmemkbuty.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fanxiaobao.xyz/Article/details/geghzddfi.sHtML

[S56] C++：optional
来源：http://wap.fanxiaobao.xyz/Article/details/gdhmmwkkm.sHtML


<!-- 参考信息 -->