代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://3g.fanxiaobao.xyz/Article/details/gbhzmsttc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fanxiaobao.xyz/Article/details/gezhprvbc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gfssjscux.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gnwlcfhbr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gdzhsdreh.sHtML

[Q90] 生成序号列
来源：http://baike.fanxiaobao.xyz/Article/details/gpiphsbae.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzkikerxf.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/ganxsjorx.sHtML

R. Bash 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gliyczmpm.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gzzovwyqw.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fanxiaobao.xyz/Article/details/gmjgcbyck.sHtML

#!/usr/bin/env bash
来源：http://blog.fanxiaobao.xyz/Article/details/gltyvsqnl.sHtML

set -euo pipefail
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjzsvweas.sHtML

[R02] 变量赋值与使用
来源：http://blog.fanxiaobao.xyz/Article/details/gunfvfxcg.sHtML

name="Tom"; echo "$name"
来源：http://wap.fanxiaobao.xyz/Article/details/gyerjoinq.sHtML

[R03] 只读变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gmxnbhvrk.sHtML

readonly PI=3.14
来源：http://read.share.fanxiaobao.xyz/Article/details/ghjlxxzjj.sHtML

[R04] 位置参数
来源：http://blog.fanxiaobao.xyz/Article/details/giixzbvrp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnrsjxxmb.sHtML

[R05] 参数默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyeawzqpd.sHtML

name="${1:-default}"
来源：http://3g.fanxiaobao.xyz/Article/details/gnnsyoaag.sHtML

[R06] 判断命令是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/geffoxddc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gygrcgnfu.sHtML

[R07] if 判断文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gvzvraddy.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gjahvrtfr.sHtML

[R08] 数值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwovnddon.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gzmmhkgmm.sHtML

[R09] 字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gumjnpsem.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gkzioywyh.sHtML

[R10] 正则匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/ggqajnqns.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gyptxcfmk.sHtML

[R11] case 多分支
来源：http://3g.fanxiaobao.xyz/Article/details/geqomveis.sHtML

case "$1" in
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggfzpltty.sHtML

start) echo "启动" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghixvxtyi.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gypnoldbf.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gwugjmacj.sHtML

esac
来源：http://www.m.share.fanxiaobao.xyz/Article/details/genjwpbli.sHtML

[R12] for 遍历文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gqkholrvo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gnhflolnp.sHtML

[R13] for 计数循环
来源：http://wap.fanxiaobao.xyz/Article/details/gsvrubprd.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gbjaturmd.sHtML

[R14] C 风格 for
来源：http://blog.fanxiaobao.xyz/Article/details/gfwkcmmfk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/geuyfyeji.sHtML

[R15] while 逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/ggobcabxm.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gjrngfkun.sHtML

[R16] until 等待条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gwgsgkcji.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/glvlmculq.sHtML

[R17] 数组定义与取值
来源：http://wap.fanxiaobao.xyz/Article/details/gmfjxugyc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsiqqldkl.sHtML

[R18] 遍历数组
来源：http://wap.fanxiaobao.xyz/Article/details/goyvhjijt.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gjvviefzm.sHtML

[R19] 数组长度
来源：http://3g.fanxiaobao.xyz/Article/details/gpcnqpqji.sHtML

echo "${#arr[@]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gnroledsq.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gstwoaelo.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gviupiqgp.sHtML

[R21] 字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gpzblvmmr.sHtML

echo "${#s}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gzapwnbaj.sHtML

[R22] 截取子串
来源：http://blog.fanxiaobao.xyz/Article/details/gqnmdwcej.sHtML

echo "${s:0:5}"
来源：http://wap.fanxiaobao.xyz/Article/details/gwxrvcdsm.sHtML

[R23] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gsrozctcs.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpshpqoks.sHtML

[R24] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gznyptxqo.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gofvptxeg.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxklnavtv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fanxiaobao.xyz/Article/details/gogvuqtrz.sHtML

[R26] 命令替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gjvsxdqop.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fanxiaobao.xyz/Article/details/gjfojvahc.sHtML

[R27] 算术展开
来源：http://wap.fanxiaobao.xyz/Article/details/gorznewbk.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fanxiaobao.xyz/Article/details/gsvwgwwai.sHtML

[R28] 浮点运算
来源：http://wap.fanxiaobao.xyz/Article/details/gtidftcjb.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghoaosrzv.sHtML

[R29] 定义函数
来源：http://3g.fanxiaobao.xyz/Article/details/gebkmgosr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fanxiaobao.xyz/Article/details/gbhcgehhf.sHtML

[R30] 函数返回状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gyavjhjze.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fanxiaobao.xyz/Article/details/gqrmbiaef.sHtML

[R31] 局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gxrgfzvgv.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsrrvmwfi.sHtML

[R32] 参数个数校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gotcumxhb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtxyhpekc.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fanxiaobao.xyz/Article/details/gvkahviez.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fanxiaobao.xyz/Article/details/gugleeang.sHtML

[R34] 退出时清理
来源：http://mobile.fanxiaobao.xyz/Article/details/glcxalobg.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjwrvijl.sHtML

[R35] 后台执行并等待
来源：http://wap.fanxiaobao.xyz/Article/details/gptsaxytf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fanxiaobao.xyz/Article/details/gixdfkrki.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gcmxvpdde.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fanxiaobao.xyz/Article/details/gvyzuylak.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqudonkxy.sHtML

files=$(ls -1)
来源：http://3g.fanxiaobao.xyz/Article/details/gvpvlgtxv.sHtML

[R38] 管道串联
来源：http://blog.fanxiaobao.xyz/Article/details/gxpfpkuxv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fanxiaobao.xyz/Article/details/gvqyjoxjr.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnbedqdvw.sHtML

cmd > out.log 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gpjhzldua.sHtML

[R40] 追加写日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gltlqakcr.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/gssqjjoho.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/gvnutayfk.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gdbmvfpmv.sHtML

[R42] 输入重定向
来源：http://mobile.fanxiaobao.xyz/Article/details/gphadbvxd.sHtML

wc -l < a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gqihtmjcq.sHtML

[R43] 按名字查找文件
来源：http://m.share.fanxiaobao.xyz/Article/details/grtiabxls.sHtML

find . -name "*.log" -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gqotxtyaz.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gytkzqtxg.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfwvadbeo.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/gbzvajjub.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fanxiaobao.xyz/Article/details/gglpoxlpa.sHtML

[R46] 递归替换文件内容
来源：http://baike.fanxiaobao.xyz/Article/details/gkvusmlqj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fanxiaobao.xyz/Article/details/guqyyyfvy.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwfcxwucm.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gosexykwm.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glmaddguv.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gyeioloma.sHtML

[R49] awk 带条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gtsbxiudm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fanxiaobao.xyz/Article/details/gwalkhqrc.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtvwbppwm.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/golseacaj.sHtML

[R51] 排序去重取前几
来源：http://blog.fanxiaobao.xyz/Article/details/getcthsxe.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fanxiaobao.xyz/Article/details/gtfxzljzu.sHtML

[R52] 统计行数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpbpwrnur.sHtML

wc -l a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gewsphjiz.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fanxiaobao.xyz/Article/details/gfqlzmdna.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/garhkxmfm.sHtML

[R54] 比较两个文件
来源：http://wap.fanxiaobao.xyz/Article/details/gxqvtacwq.sHtML

diff a.txt b.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/grmqkfoie.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/gionjvxtv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fanxiaobao.xyz/Article/details/gjfopopha.sHtML

[R56] 远程拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gqlprsess.sHtML

scp file user@host:/path/
来源：http://3g.fanxiaobao.xyz/Article/details/guhnstnxl.sHtML

[R57] 远程执行命令
来源：http://wap.fanxiaobao.xyz/Article/details/gtsuznzlg.sHtML

ssh user@host 'uptime'
来源：http://m.share.fanxiaobao.xyz/Article/details/gxnuxmhng.sHtML

[R58] 下载文件
来源：http://3g.fanxiaobao.xyz/Article/details/gkdfjonef.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxgferohn.sHtML

[R59] 发 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gbpjoijdi.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjziljsm.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gqswzrnxw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fanxiaobao.xyz/Article/details/grucbsixh.sHtML

[R61] 磁盘占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/goivncatl.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/gzekumonb.sHtML

[R62] 找最占空间的文件
来源：http://baike.fanxiaobao.xyz/Article/details/gmlstobql.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fanxiaobao.xyz/Article/details/ggvdoksrh.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gtgkgmkes.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fanxiaobao.xyz/Article/details/gvzarocxi.sHtML

[R64] 结束进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gabnqtwbv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnhirbbdy.sHtML

[R65] 查看端口占用
来源：http://baike.fanxiaobao.xyz/Article/details/ggztrrdwv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fanxiaobao.xyz/Article/details/gmnhvdsrw.sHtML

[R66] 定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/gvdhrsuup.sHtML

crontab -e;  crontab -l
来源：http://wap.fanxiaobao.xyz/Article/details/gytqueylr.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fanxiaobao.xyz/Article/details/gbboojxbi.sHtML

openssl rand -hex 16
来源：http://baike.fanxiaobao.xyz/Article/details/gpfywfmpt.sHtML

[R68] 计算文件校验值
来源：http://wap.fanxiaobao.xyz/Article/details/grqlkadic.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gyrkajzgf.sHtML

[R69] 生成随机密码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbdleylhr.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fanxiaobao.xyz/Article/details/ghbjlgecn.sHtML

[R70] 时间戳与互转
来源：http://read.share.fanxiaobao.xyz/Article/details/gvsfxeeew.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fanxiaobao.xyz/Article/details/gqrxgvscf.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gnrqjyyhb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fanxiaobao.xyz/Article/details/gplctowbh.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqfllqzy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gbmslbyzi.sHtML

[R73] 分割大日志
来源：http://wap.fanxiaobao.xyz/Article/details/gnfundysx.sHtML

split -l 1000 big.log part_
来源：http://www.share.fanxiaobao.xyz/Article/details/gzchghatj.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkqvrnsvp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gfqwhfpku.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gydvlbmnv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fanxiaobao.xyz/Article/details/gizougwzp.sHtML

[R76] 使用临时文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gllrwsotv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gizxidhkx.sHtML

[R77] 读取用户输入
来源：http://3g.fanxiaobao.xyz/Article/details/ganzqhpcf.sHtML

read -rp "请输入: " ans
来源：http://baike.fanxiaobao.xyz/Article/details/gobrrhepj.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsluhnpfb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gflblhqrk.sHtML

[R79] 解析命令行选项
来源：http://read.share.fanxiaobao.xyz/Article/details/girncqfip.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsmlznlkx.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjlnblxaf.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/gmgwbulqx.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtrjuxocw.sHtML

S. C / C++ 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gbnoneobt.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gskwfadcc.sHtML

[S01] C：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbydoiua.sHtML

#include <stdio.h>
来源：http://baike.fanxiaobao.xyz/Article/details/gmniuhwxn.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fanxiaobao.xyz/Article/details/gyvuhcdmg.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gowxbpjjl.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxooyufws.sHtML

[S03] C：读入整数
来源：http://m.share.fanxiaobao.xyz/Article/details/guydhpwyh.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqwqxexxn.sHtML

[S04] C：字符串复制
来源：http://www.share.fanxiaobao.xyz/Article/details/gowixldke.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/gbvlnxosw.sHtML

[S05] C：字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/geqpatled.sHtML

strlen(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxivseinp.sHtML

[S06] C：字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gqggoaahq.sHtML

strcmp(a, b) == 0
来源：http://baike.fanxiaobao.xyz/Article/details/gzxtozbdy.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gdtkaevjp.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gflojbjjt.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/gytmojmur.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gporvjoks.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyxuzelzr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyucqrtcg.sHtML

[S10] C：指针与解引用
来源：http://www.share.fanxiaobao.xyz/Article/details/gnsyoxdlx.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gxcozjcjw.sHtML

[S11] C：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gbrpmcgrd.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fanxiaobao.xyz/Article/details/gujgdccwm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvqsgzeyr.sHtML

fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghhxjegjr.sHtML

[S12] C：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdauexmon.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkoktwmrh.sHtML

[S13] C：宏定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxoizjuo.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fanxiaobao.xyz/Article/details/gdcywodko.sHtML

[S14] C：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvdgmhyq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fanxiaobao.xyz/Article/details/gxopsaffk.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyklexifw.sHtML

(double) a / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gjizfrfch.sHtML

[S16] C：位操作置位
来源：http://3g.fanxiaobao.xyz/Article/details/gawnicsbh.sHtML

x |= (1 << 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gksrmlgwc.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvnhanvf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fanxiaobao.xyz/Article/details/gqtyvozin.sHtML

[S18] C：命令行参数
来源：http://wap.fanxiaobao.xyz/Article/details/gubywyali.sHtML

int main(int argc, char **argv)
来源：http://baike.fanxiaobao.xyz/Article/details/ggjmlxnar.sHtML

[S19] C：快速排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gvthqwrcz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gxdlcekqa.sHtML

[S20] C：二分查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gnydwbbzs.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/grevqpumx.sHtML

[S21] C：字符类别判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gnaxwllko.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gniovegpd.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzuwcryd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fanxiaobao.xyz/Article/details/gqtahclsj.sHtML

[S23] C：随机数
来源：http://blog.fanxiaobao.xyz/Article/details/gscmyvcyc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gpkuhtozw.sHtML

[S24] C：获取本地时间
来源：http://3g.fanxiaobao.xyz/Article/details/gwcqkwxml.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fanxiaobao.xyz/Article/details/grxrnagfv.sHtML

[S25] C：内存拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gnjodpfmw.sHtML

memcpy(dst, src, n);
来源：http://blog.fanxiaobao.xyz/Article/details/gprevaoxc.sHtML

[S26] C：内存清零
来源：http://m.share.fanxiaobao.xyz/Article/details/gopcssukj.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gihhkxuzf.sHtML

[S27] C：定义常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gfkpakpcl.sHtML

const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gtkakdsmo.sHtML

[S28] C：静态变量
来源：http://blog.fanxiaobao.xyz/Article/details/ghvlsbpon.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmpmlqjnw.sHtML

[S29] C：变参函数
来源：http://baike.fanxiaobao.xyz/Article/details/gaxykgwqo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkywivnpi.sHtML

[S30] C：头文件保护
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggxssxigk.sHtML

#ifndef X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gbghqktcc.sHtML

#define X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gogurleiz.sHtML

#endif
来源：http://read.share.fanxiaobao.xyz/Article/details/gqrrslkzk.sHtML

[S31] C++：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gibvsiliy.sHtML

#include <iostream>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxhcdnpgp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzflzqedb.sHtML

[S32] C++：字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqixvpjtg.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fanxiaobao.xyz/Article/details/grjdbvmnu.sHtML

[S33] C++：vector 增删
来源：http://blog.fanxiaobao.xyz/Article/details/gvzvhwyku.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/genynmhse.sHtML

[S34] C++：遍历 vector
来源：http://3g.fanxiaobao.xyz/Article/details/gzvcpkyru.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsuribmbr.sHtML

[S35] C++：map
来源：http://read.share.fanxiaobao.xyz/Article/details/gfjrxxcgm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/glrfbckan.sHtML

[S36] C++：unordered_map
来源：http://wap.fanxiaobao.xyz/Article/details/gzmchvmuh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdzzohinr.sHtML

[S37] C++：set
来源：http://baike.fanxiaobao.xyz/Article/details/gnfptylmt.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gxmsrszro.sHtML

[S38] C++：排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnvwcplct.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gtbubguhq.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fanxiaobao.xyz/Article/details/ggetnzvek.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fanxiaobao.xyz/Article/details/gswaawrez.sHtML

[S40] C++：查找元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gqmdntfdw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gihfakoin.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdpccdfyp.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gulhfvuiw.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gwzgbcxcs.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fanxiaobao.xyz/Article/details/gnzbdgkyw.sHtML

[S43] C++：智能指针
来源：http://wap.fanxiaobao.xyz/Article/details/gwefymypi.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fanxiaobao.xyz/Article/details/giutlprtj.sHtML

[S44] C++：引用传参
来源：http://www.share.fanxiaobao.xyz/Article/details/gastufeae.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjfoxhlbo.sHtML

[S45] C++：lambda
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtnovkkoy.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fanxiaobao.xyz/Article/details/gvtrvneas.sHtML

[S46] C++：函数模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gglprlpiy.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gsrirdygl.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gxligynca.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fanxiaobao.xyz/Article/details/gnjspyhwv.sHtML

[S48] C++：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gxlvgpcmi.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fanxiaobao.xyz/Article/details/gwbuvhrdl.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guulclypf.sHtML

[S49] C++：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gcpzqvqrz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gxbqyvavt.sHtML

[S50] C++：格式化数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gvfrpnvob.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gbjomdqlx.sHtML

[S51] C++：显式类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gyhbxmdhm.sHtML

static_cast<double>(a) / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gupkpnqee.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fanxiaobao.xyz/Article/details/ggtxtbxyc.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fanxiaobao.xyz/Article/details/gkdjcjniv.sHtML

[S53] C++：移动语义
来源：http://www.share.fanxiaobao.xyz/Article/details/gjozdemrf.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fanxiaobao.xyz/Article/details/gcgqiuuci.sHtML

[S54] C++：异常处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gxabbmzzy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcmkoschv.sHtML

[S55] C++：结构化绑定
来源：http://baike.fanxiaobao.xyz/Article/details/gxrkogrqi.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gceoejbmq.sHtML

[S56] C++：optional
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gewasekmu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzxluquq.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjisqhrnf.sHtML

constexpr int N = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gkrrtkwqb.sHtML

[S58] C++：命名空间
来源：http://3g.fanxiaobao.xyz/Article/details/guzthoazf.sHtML


<!-- 参考信息 -->