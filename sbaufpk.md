代发 wailian999

[Q82] 字符长度与字节长度
来源：http://www.blog.hesvh.cn/Article/details/gickqbnqn.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/ggsxxarjb.sHtML

[Q83] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/ghklwatmv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gaudpasys.sHtML

[Q84] 去除首尾空格
来源：http://mobile.zdbjq.cn/Article/details/gyteieksk.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gxioyflxk.sHtML

[Q85] 数值取整
来源：http://read.share.zdbjq.cn/Article/details/garbmyogw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.hesvh.cn/Article/details/gvuryttnq.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.hesvh.cn/Article/details/gcziqlhrg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fehbvm.com/Article/details/gxfhomycy.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.zdbjq.cn/Article/details/gzttniaxl.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fehbvm.com/Article/details/grfjrqawq.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.zdbjq.cn/Article/details/gjtdvbulk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.zdbjq.cn/Article/details/gevrepenk.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.hesvh.cn/Article/details/gwcvuicik.sHtML

[Q89] 判断表是否存在
来源：http://baike.zdbjq.cn/Article/details/gkcttabgw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.hesvh.cn/Article/details/ghkfbuyec.sHtML

[Q90] 生成序号列
来源：http://wap.fehbvm.com/Article/details/gqyxgljmv.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.zdbjq.cn/Article/details/gtqgkfxnk.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gmckrsknf.sHtML

R. Bash 专题
来源：http://m.share.fehbvm.com/Article/details/gjbhyivzv.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gvnipqrkb.sHtML

[R01] shebang 与严格模式
来源：http://blog.fehbvm.com/Article/details/gtdltjyhn.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fehbvm.com/Article/details/grskkofqb.sHtML

set -euo pipefail
来源：http://3g.fehbvm.com/Article/details/garyljacq.sHtML

[R02] 变量赋值与使用
来源：http://blog.fehbvm.com/Article/details/gonzskxlj.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.zdbjq.cn/Article/details/gvlutnyal.sHtML

[R03] 只读变量
来源：http://www.share.hesvh.cn/Article/details/gzjgugblu.sHtML

readonly PI=3.14
来源：http://baike.zdbjq.cn/Article/details/gxxrtreur.sHtML

[R04] 位置参数
来源：http://www.m.share.fehbvm.com/Article/details/gdnizeodl.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.hesvh.cn/Article/details/gfpkjvfwy.sHtML

[R05] 参数默认值
来源：http://www.m.share.hesvh.cn/Article/details/gfsnbralj.sHtML

name="${1:-default}"
来源：http://mobile.hesvh.cn/Article/details/gsxnnzeem.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.hesvh.cn/Article/details/gzdyzixhu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/ggkzniucz.sHtML

[R07] if 判断文件
来源：http://m.share.fehbvm.com/Article/details/gksramphe.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.hesvh.cn/Article/details/ghpepepej.sHtML

[R08] 数值比较
来源：http://www.blog.zdbjq.cn/Article/details/ggrwuohut.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fehbvm.com/Article/details/gnyyoqhzq.sHtML

[R09] 字符串比较
来源：http://wap.zdbjq.cn/Article/details/gcxzegemx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.hesvh.cn/Article/details/gvrihsold.sHtML

[R10] 正则匹配
来源：http://wap.zdbjq.cn/Article/details/gskhlbpgf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fehbvm.com/Article/details/geqaoewrq.sHtML

[R11] case 多分支
来源：http://wap.fehbvm.com/Article/details/glhbahnss.sHtML

case "$1" in
来源：http://wap.zdbjq.cn/Article/details/gwwaympij.sHtML

start) echo "启动" ;;
来源：http://www.blog.zdbjq.cn/Article/details/ghrzbchlu.sHtML

stop)  echo "停止" ;;
来源：http://baike.zdbjq.cn/Article/details/glfbptnyb.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.hesvh.cn/Article/details/gsktwdkeg.sHtML

esac
来源：http://m.share.hesvh.cn/Article/details/guvjfboej.sHtML

[R12] for 遍历文件
来源：http://www.blog.zdbjq.cn/Article/details/giazivdhs.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.zdbjq.cn/Article/details/goysnvulm.sHtML

[R13] for 计数循环
来源：http://www.m.share.hesvh.cn/Article/details/glvpjzjhu.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fehbvm.com/Article/details/gxjvvdxhl.sHtML

[R14] C 风格 for
来源：http://www.blog.zdbjq.cn/Article/details/gpqinoexf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gkoezkctj.sHtML

[R15] while 逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gnczzmcoi.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fehbvm.com/Article/details/gwjeanlub.sHtML

[R16] until 等待条件
来源：http://blog.fehbvm.com/Article/details/giltprtss.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/gmheutpvi.sHtML

[R17] 数组定义与取值
来源：http://m.share.fehbvm.com/Article/details/gbyspbmmn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.zdbjq.cn/Article/details/gsrzhmmgn.sHtML

[R18] 遍历数组
来源：http://mobile.zdbjq.cn/Article/details/geozluoxi.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.hesvh.cn/Article/details/gtvsgzcgs.sHtML

[R19] 数组长度
来源：http://baike.fehbvm.com/Article/details/gchmetbxk.sHtML

echo "${#arr[@]}"
来源：http://read.share.zdbjq.cn/Article/details/ghmgujwjk.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.zdbjq.cn/Article/details/gvaepuhoy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.zdbjq.cn/Article/details/gvodfoupn.sHtML

[R21] 字符串长度
来源：http://3g.hesvh.cn/Article/details/gnblwamec.sHtML

echo "${#s}"
来源：http://mobile.fehbvm.com/Article/details/gtzfyulix.sHtML

[R22] 截取子串
来源：http://www.share.hesvh.cn/Article/details/ghnslaryf.sHtML

echo "${s:0:5}"
来源：http://blog.zdbjq.cn/Article/details/gmakadbmo.sHtML

[R23] 字符串替换
来源：http://read.share.fehbvm.com/Article/details/gohzcueln.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.hesvh.cn/Article/details/ghnnsyefj.sHtML

[R24] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gjaemjlcn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.hesvh.cn/Article/details/gwlxgymkr.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fehbvm.com/Article/details/gukycbppx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.zdbjq.cn/Article/details/goxhfkzip.sHtML

[R26] 命令替换
来源：http://m.share.fehbvm.com/Article/details/grmzsupyl.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fehbvm.com/Article/details/glqrqbvhy.sHtML

[R27] 算术展开
来源：http://read.share.fehbvm.com/Article/details/gmdlcovmm.sHtML

echo $((1 + 2 * 3))
来源：http://3g.zdbjq.cn/Article/details/geidjinrv.sHtML

[R28] 浮点运算
来源：http://m.share.fehbvm.com/Article/details/gjtcdbqmp.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fehbvm.com/Article/details/gtjcmaguw.sHtML

[R29] 定义函数
来源：http://read.share.hesvh.cn/Article/details/gycdwaflf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.zdbjq.cn/Article/details/galyildqx.sHtML

[R30] 函数返回状态码
来源：http://blog.fehbvm.com/Article/details/gpyeuzzll.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.hesvh.cn/Article/details/guaelnwcy.sHtML

[R31] 局部变量
来源：http://read.share.fehbvm.com/Article/details/gxwvujhbc.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fehbvm.com/Article/details/gxxigywnj.sHtML

[R32] 参数个数校验
来源：http://blog.hesvh.cn/Article/details/gvxqjfdvv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/gyvdelopn.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.zdbjq.cn/Article/details/gnqwbrgwm.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.hesvh.cn/Article/details/gmavoozkm.sHtML

[R34] 退出时清理
来源：http://read.share.zdbjq.cn/Article/details/gxyerpdgn.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/gduileeuv.sHtML

[R35] 后台执行并等待
来源：http://wap.zdbjq.cn/Article/details/gdlbpkylk.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fehbvm.com/Article/details/gzizrfmpy.sHtML

[R36] 并发执行多个任务
来源：http://wap.hesvh.cn/Article/details/geeibexhl.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.zdbjq.cn/Article/details/gmyvoodbk.sHtML

[R37] 把输出赋给变量
来源：http://wap.fehbvm.com/Article/details/gxylsywge.sHtML

files=$(ls -1)
来源：http://www.blog.hesvh.cn/Article/details/gefvwonai.sHtML

[R38] 管道串联
来源：http://www.share.fehbvm.com/Article/details/geleawgkw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fehbvm.com/Article/details/gghbpxcir.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.zdbjq.cn/Article/details/gmveppold.sHtML

cmd > out.log 2>&1
来源：http://wap.hesvh.cn/Article/details/gzhvfrcas.sHtML

[R40] 追加写日志
来源：http://read.share.hesvh.cn/Article/details/gdqgweqbd.sHtML

echo "log" >> out.log
来源：http://www.m.share.hesvh.cn/Article/details/guchkuclm.sHtML

[R41] 丢弃输出
来源：http://blog.fehbvm.com/Article/details/gxrmrgbbs.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fehbvm.com/Article/details/grjhgpeua.sHtML

[R42] 输入重定向
来源：http://mobile.zdbjq.cn/Article/details/guyqgmcyy.sHtML

wc -l < a.txt
来源：http://www.m.share.hesvh.cn/Article/details/ghwtkepeb.sHtML

[R43] 按名字查找文件
来源：http://www.blog.hesvh.cn/Article/details/gkrzjxsoz.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.hesvh.cn/Article/details/gudhckwne.sHtML

[R44] 按修改时间查找
来源：http://wap.hesvh.cn/Article/details/grfpcgfdg.sHtML

find . -mtime -7 -type f
来源：http://baike.zdbjq.cn/Article/details/gnlpesdkn.sHtML

[R45] 批量删除
来源：http://m.share.fehbvm.com/Article/details/gulkvbfwy.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fehbvm.com/Article/details/gmkdimggp.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fehbvm.com/Article/details/gnwjztbgx.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fehbvm.com/Article/details/gyvjnfkji.sHtML

[R47] sed 单行替换
来源：http://3g.hesvh.cn/Article/details/gbezzmzia.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.hesvh.cn/Article/details/gucacqqln.sHtML

[R48] awk 取指定列
来源：http://3g.hesvh.cn/Article/details/gebjdupqn.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.hesvh.cn/Article/details/gjaatvgdn.sHtML

[R49] awk 带条件
来源：http://www.blog.fehbvm.com/Article/details/gtmfriwuv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fehbvm.com/Article/details/guykqlydq.sHtML

[R50] awk 求和
来源：http://mobile.fehbvm.com/Article/details/gyrkshehm.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.hesvh.cn/Article/details/gcbyubryp.sHtML

[R51] 排序去重取前几
来源：http://baike.zdbjq.cn/Article/details/gqdakmafj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fehbvm.com/Article/details/gzgbvtczu.sHtML

[R52] 统计行数
来源：http://blog.fehbvm.com/Article/details/gwdxeymge.sHtML

wc -l a.txt
来源：http://www.blog.hesvh.cn/Article/details/ghovhkzwx.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fehbvm.com/Article/details/gleyroesk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.zdbjq.cn/Article/details/guqlgkwhx.sHtML

[R54] 比较两个文件
来源：http://blog.zdbjq.cn/Article/details/geboysrzm.sHtML

diff a.txt b.txt
来源：http://blog.hesvh.cn/Article/details/gblzuixml.sHtML

[R55] 压缩与解压
来源：http://baike.fehbvm.com/Article/details/gnsiuikiw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.hesvh.cn/Article/details/gbcyoumom.sHtML

[R56] 远程拷贝
来源：http://blog.zdbjq.cn/Article/details/gdmcfqgho.sHtML

scp file user@host:/path/
来源：http://mobile.fehbvm.com/Article/details/gffjtpnzd.sHtML

[R57] 远程执行命令
来源：http://www.blog.hesvh.cn/Article/details/grjppprsl.sHtML

ssh user@host 'uptime'
来源：http://blog.hesvh.cn/Article/details/gbjyghihz.sHtML

[R58] 下载文件
来源：http://mobile.fehbvm.com/Article/details/gfrbrziep.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.hesvh.cn/Article/details/gsvwbraku.sHtML

[R59] 发 POST JSON
来源：http://baike.zdbjq.cn/Article/details/gwtpjqcwe.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.zdbjq.cn/Article/details/gleehzcfo.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/gmwcegvaq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.hesvh.cn/Article/details/gtenipnyh.sHtML

[R61] 磁盘占用
来源：http://www.share.zdbjq.cn/Article/details/gygxwtkbt.sHtML

df -h;  du -sh *
来源：http://www.blog.hesvh.cn/Article/details/garvkbdch.sHtML

[R62] 找最占空间的文件
来源：http://m.share.zdbjq.cn/Article/details/ghwqqjauc.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fehbvm.com/Article/details/gkztdpcmi.sHtML

[R63] 内存与进程
来源：http://blog.hesvh.cn/Article/details/gcrytzfaz.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fehbvm.com/Article/details/gffshzheb.sHtML

[R64] 结束进程
来源：http://www.blog.fehbvm.com/Article/details/gbboigikp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fehbvm.com/Article/details/gnrgebomc.sHtML

[R65] 查看端口占用
来源：http://read.share.fehbvm.com/Article/details/goxqfazwf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.hesvh.cn/Article/details/ghptsalik.sHtML

[R66] 定时任务
来源：http://wap.zdbjq.cn/Article/details/gnzruxqqu.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.hesvh.cn/Article/details/gexgticrt.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fehbvm.com/Article/details/gpnrbuosn.sHtML

openssl rand -hex 16
来源：http://baike.fehbvm.com/Article/details/gvngdfoby.sHtML

[R68] 计算文件校验值
来源：http://wap.zdbjq.cn/Article/details/gpqtpueky.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fehbvm.com/Article/details/ghjzwueqg.sHtML

[R69] 生成随机密码
来源：http://3g.hesvh.cn/Article/details/glvsvjoup.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.hesvh.cn/Article/details/gyrypltgf.sHtML

[R70] 时间戳与互转
来源：http://blog.hesvh.cn/Article/details/gpkkzmgpt.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.hesvh.cn/Article/details/gdtdlqrdt.sHtML

[R71] 日期格式化
来源：http://baike.fehbvm.com/Article/details/gvzjojlkp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.hesvh.cn/Article/details/gteezeovu.sHtML

[R72] 等待端口就绪
来源：http://mobile.zdbjq.cn/Article/details/gtbnktmci.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/gaqxsjtqv.sHtML

[R73] 分割大日志
来源：http://www.m.share.zdbjq.cn/Article/details/gwlffiqai.sHtML

split -l 1000 big.log part_
来源：http://3g.fehbvm.com/Article/details/gslsejqqg.sHtML

[R74] 批量重命名
来源：http://read.share.fehbvm.com/Article/details/gbiniokbj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.zdbjq.cn/Article/details/gevjvvoff.sHtML

[R75] 导出环境变量
来源：http://read.share.hesvh.cn/Article/details/gfwrrfffu.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.zdbjq.cn/Article/details/girinllmn.sHtML

[R76] 使用临时文件
来源：http://www.blog.fehbvm.com/Article/details/gshutzbyb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gdesdfpcy.sHtML

[R77] 读取用户输入
来源：http://blog.fehbvm.com/Article/details/gffjaebfu.sHtML

read -rp "请输入: " ans
来源：http://3g.zdbjq.cn/Article/details/gfptdumcr.sHtML

[R78] 交互式菜单
来源：http://www.blog.zdbjq.cn/Article/details/giudljjuc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fehbvm.com/Article/details/gztjgnfdl.sHtML

[R79] 解析命令行选项
来源：http://www.share.hesvh.cn/Article/details/gwnpowteu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.zdbjq.cn/Article/details/guqyghlcm.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.hesvh.cn/Article/details/gxwjsmqbq.sHtML

time ./run.sh
来源：http://wap.zdbjq.cn/Article/details/ghkhkpyjm.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gbemyhvym.sHtML

S. C / C++ 专题
来源：http://www.blog.hesvh.cn/Article/details/gtjydghvj.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gvoatsxnf.sHtML

[S01] C：Hello World
来源：http://m.share.fehbvm.com/Article/details/gwloddhzy.sHtML

#include <stdio.h>
来源：http://baike.fehbvm.com/Article/details/gfjtcawrw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.hesvh.cn/Article/details/gdjnblpin.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.zdbjq.cn/Article/details/gouqrzaco.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.hesvh.cn/Article/details/geolreilv.sHtML

[S03] C：读入整数
来源：http://www.share.zdbjq.cn/Article/details/gsfxbgotd.sHtML

int x; scanf("%d", &x);
来源：http://baike.zdbjq.cn/Article/details/gvxodnqwz.sHtML

[S04] C：字符串复制
来源：http://m.share.fehbvm.com/Article/details/ghfblkhar.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fehbvm.com/Article/details/gkacwxapp.sHtML

[S05] C：字符串长度
来源：http://blog.hesvh.cn/Article/details/grauiuzwj.sHtML

strlen(s)
来源：http://www.share.zdbjq.cn/Article/details/gwoecgsqc.sHtML

[S06] C：字符串比较
来源：http://m.share.hesvh.cn/Article/details/gazsirayh.sHtML

strcmp(a, b) == 0
来源：http://www.blog.hesvh.cn/Article/details/ghdipzrul.sHtML

[S07] C：数组遍历求和
来源：http://www.share.zdbjq.cn/Article/details/gahhrxlgz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.hesvh.cn/Article/details/gyrghcysj.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.zdbjq.cn/Article/details/gapfhmlyg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.zdbjq.cn/Article/details/gnmhdzevt.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.hesvh.cn/Article/details/gfynuuwkq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.zdbjq.cn/Article/details/ggjtwvtoz.sHtML

[S10] C：指针与解引用
来源：http://3g.hesvh.cn/Article/details/gtowqitag.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fehbvm.com/Article/details/gcsqivcmv.sHtML

[S11] C：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gbgvxbkzp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fehbvm.com/Article/details/gassewbza.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.zdbjq.cn/Article/details/gfuqmtpnm.sHtML

fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/ghjockdfo.sHtML

[S12] C：写文件
来源：http://blog.zdbjq.cn/Article/details/gzasszwvn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.hesvh.cn/Article/details/gutgxafnt.sHtML

[S13] C：宏定义
来源：http://m.share.fehbvm.com/Article/details/gsmqkrpca.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fehbvm.com/Article/details/giprmgmje.sHtML

[S14] C：枚举
来源：http://www.share.zdbjq.cn/Article/details/gxdfkakeh.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.hesvh.cn/Article/details/gbagsmsjl.sHtML

[S15] C：类型转换
来源：http://wap.hesvh.cn/Article/details/gkghfstxy.sHtML

(double) a / b
来源：http://m.share.fehbvm.com/Article/details/gaextluvz.sHtML

[S16] C：位操作置位
来源：http://www.share.zdbjq.cn/Article/details/gueupiegv.sHtML

x |= (1 << 3);
来源：http://blog.fehbvm.com/Article/details/giqekditm.sHtML

[S17] C：安全拼接字符串
来源：http://3g.hesvh.cn/Article/details/gexfypgnm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.hesvh.cn/Article/details/gycqfmmfr.sHtML

[S18] C：命令行参数
来源：http://baike.zdbjq.cn/Article/details/gohkrnnue.sHtML

int main(int argc, char **argv)
来源：http://www.share.hesvh.cn/Article/details/gluertsem.sHtML

[S19] C：快速排序
来源：http://3g.fehbvm.com/Article/details/grzuzwkzj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/gmkqdqebu.sHtML

[S20] C：二分查找
来源：http://3g.zdbjq.cn/Article/details/ghxmuaokp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gtjaxlrbl.sHtML

[S21] C：字符类别判断
来源：http://wap.hesvh.cn/Article/details/gnwnwxaym.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.hesvh.cn/Article/details/gfzvfnmkm.sHtML

[S22] C：字符串转数字
来源：http://www.blog.hesvh.cn/Article/details/gvhagftps.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fehbvm.com/Article/details/gndomueps.sHtML

[S23] C：随机数
来源：http://wap.hesvh.cn/Article/details/gyumrkxob.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fehbvm.com/Article/details/gkzujewlg.sHtML

[S24] C：获取本地时间
来源：http://wap.hesvh.cn/Article/details/gejstqtgv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fehbvm.com/Article/details/gmeujtbvo.sHtML

[S25] C：内存拷贝
来源：http://www.blog.zdbjq.cn/Article/details/ggayvhopj.sHtML

memcpy(dst, src, n);
来源：http://www.blog.hesvh.cn/Article/details/gjcupaomn.sHtML

[S26] C：内存清零
来源：http://3g.fehbvm.com/Article/details/ghzbfesuf.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fehbvm.com/Article/details/gknlkfunt.sHtML

[S27] C：定义常量
来源：http://m.share.hesvh.cn/Article/details/gbsgdxmku.sHtML

const double PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gzbjigedy.sHtML

[S28] C：静态变量
来源：http://blog.hesvh.cn/Article/details/gkmtnwfru.sHtML

static int counter = 0;
来源：http://3g.hesvh.cn/Article/details/gbawisgiv.sHtML

[S29] C：变参函数
来源：http://baike.zdbjq.cn/Article/details/gzdgmshuo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.hesvh.cn/Article/details/gjkchrzut.sHtML

[S30] C：头文件保护
来源：http://blog.fehbvm.com/Article/details/gajnjuvsn.sHtML

#ifndef X_H
来源：http://baike.hesvh.cn/Article/details/gajewkqlx.sHtML

#define X_H
来源：http://m.share.hesvh.cn/Article/details/ggafizpsf.sHtML

#endif
来源：http://3g.zdbjq.cn/Article/details/guuxsehoi.sHtML

[S31] C++：Hello World
来源：http://wap.zdbjq.cn/Article/details/gbxkpvnxt.sHtML

#include <iostream>
来源：http://read.share.fehbvm.com/Article/details/gjiprpnbd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.zdbjq.cn/Article/details/gdnetnptk.sHtML

[S32] C++：字符串
来源：http://baike.zdbjq.cn/Article/details/gvnmzmqkb.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fehbvm.com/Article/details/gklcdabex.sHtML

[S33] C++：vector 增删
来源：http://m.share.fehbvm.com/Article/details/gjaeeztni.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fehbvm.com/Article/details/gdhytvkht.sHtML

[S34] C++：遍历 vector
来源：http://3g.fehbvm.com/Article/details/gfdkznxsn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.hesvh.cn/Article/details/gkhxffeay.sHtML

[S35] C++：map
来源：http://3g.zdbjq.cn/Article/details/gnktlxemy.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/gjzaewjny.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fehbvm.com/Article/details/gvortxfgh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gdfhjbzjr.sHtML

[S37] C++：set
来源：http://3g.zdbjq.cn/Article/details/gkxtikrpk.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fehbvm.com/Article/details/gpmpcgjla.sHtML

[S38] C++：排序
来源：http://m.share.hesvh.cn/Article/details/ghzteipor.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fehbvm.com/Article/details/grcbeulda.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.hesvh.cn/Article/details/gzndjvhnu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.zdbjq.cn/Article/details/gpaidwlfw.sHtML

[S40] C++：查找元素
来源：http://www.m.share.zdbjq.cn/Article/details/gebhminxb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.hesvh.cn/Article/details/gvkglgmgz.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fehbvm.com/Article/details/ghmprmsbf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fehbvm.com/Article/details/gvcrtwgso.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fehbvm.com/Article/details/gxrpuedsg.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.hesvh.cn/Article/details/gwpiymfxo.sHtML

[S43] C++：智能指针
来源：http://m.share.zdbjq.cn/Article/details/goihebfld.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.hesvh.cn/Article/details/gofvrcbfw.sHtML

[S44] C++：引用传参
来源：http://m.share.fehbvm.com/Article/details/grkzapiea.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fehbvm.com/Article/details/gugkfacqr.sHtML

[S45] C++：lambda
来源：http://baike.zdbjq.cn/Article/details/gpfgcueih.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.hesvh.cn/Article/details/gjlqznpdd.sHtML

[S46] C++：函数模板
来源：http://www.blog.zdbjq.cn/Article/details/gklcfjyql.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.hesvh.cn/Article/details/glompsmcj.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fehbvm.com/Article/details/gipcuqqps.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fehbvm.com/Article/details/gyfgrrlrz.sHtML

[S48] C++：逐行读文件
来源：http://blog.hesvh.cn/Article/details/guxtbjtwt.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fehbvm.com/Article/details/ghzqhfcqm.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.hesvh.cn/Article/details/guinqppky.sHtML

[S49] C++：写文件
来源：http://blog.fehbvm.com/Article/details/gvncxnjyo.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fehbvm.com/Article/details/gtjtaobxe.sHtML

[S50] C++：格式化数字
来源：http://wap.hesvh.cn/Article/details/gmwtjkyyv.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/guqfyrgjk.sHtML

[S51] C++：显式类型转换
来源：http://m.share.hesvh.cn/Article/details/gefrgvdxg.sHtML

static_cast<double>(a) / b
来源：http://wap.hesvh.cn/Article/details/gotgzefwe.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.zdbjq.cn/Article/details/gudbhbign.sHtML


<!-- 参考信息 -->