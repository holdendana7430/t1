代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://blog.fanxiaobao.xyz/Article/details/gknrwxuam.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fanxiaobao.xyz/Article/details/gploxxxla.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gixccjsts.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxlyffgp.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gpkjgpdbp.sHtML

[Q90] 生成序号列
来源：http://read.share.fanxiaobao.xyz/Article/details/gvfydkvux.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkptkdtvm.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/goighvrol.sHtML

R. Bash 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gzwibuaqm.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gydrbwuqf.sHtML

[R01] shebang 与严格模式
来源：http://blog.fanxiaobao.xyz/Article/details/gnjnnscuz.sHtML

#!/usr/bin/env bash
来源：http://3g.fanxiaobao.xyz/Article/details/ghkzlcrsg.sHtML

set -euo pipefail
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjajfiao.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fanxiaobao.xyz/Article/details/gxabtwvma.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfaarekyu.sHtML

[R03] 只读变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmhzjrha.sHtML

readonly PI=3.14
来源：http://mobile.fanxiaobao.xyz/Article/details/gdikthqmb.sHtML

[R04] 位置参数
来源：http://baike.fanxiaobao.xyz/Article/details/goiiesrhz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fanxiaobao.xyz/Article/details/gkpdxcnwl.sHtML

[R05] 参数默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/gxewnrihi.sHtML

name="${1:-default}"
来源：http://3g.fanxiaobao.xyz/Article/details/gqpqrilqs.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gyiparqzt.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/giztfelns.sHtML

[R07] if 判断文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gobatxoig.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gpvtavgxb.sHtML

[R08] 数值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gczxakyuj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gnvrpogus.sHtML

[R09] 字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gnljxcdeg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gkbpxvnny.sHtML

[R10] 正则匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/grtcoxmmo.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/ggdsrdbee.sHtML

[R11] case 多分支
来源：http://3g.fanxiaobao.xyz/Article/details/gzquyhwai.sHtML

case "$1" in
来源：http://blog.fanxiaobao.xyz/Article/details/gzttqaqkv.sHtML

start) echo "启动" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvkjgowhj.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/galirlpag.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvmqngoh.sHtML

esac
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpjhkyqua.sHtML

[R12] for 遍历文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gyztdoprw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gujvhaxqv.sHtML

[R13] for 计数循环
来源：http://read.share.fanxiaobao.xyz/Article/details/guqynpzip.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gzigqwgdr.sHtML

[R14] C 风格 for
来源：http://mobile.fanxiaobao.xyz/Article/details/gpkzoyyxv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcswiudza.sHtML

[R15] while 逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gzaoyurha.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gsbikjjus.sHtML

[R16] until 等待条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gqpqgdlpc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gcuwhlnoj.sHtML

[R17] 数组定义与取值
来源：http://mobile.fanxiaobao.xyz/Article/details/gbpiasgkz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gpyrwtpdg.sHtML

[R18] 遍历数组
来源：http://read.share.fanxiaobao.xyz/Article/details/gyojkxpwz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/grdphvxzm.sHtML

[R19] 数组长度
来源：http://wap.fanxiaobao.xyz/Article/details/gjjhidtfs.sHtML

echo "${#arr[@]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/glvzrhlzp.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fanxiaobao.xyz/Article/details/gvczcrybh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fanxiaobao.xyz/Article/details/ggcuocuhm.sHtML

[R21] 字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gzyqierpc.sHtML

echo "${#s}"
来源：http://wap.fanxiaobao.xyz/Article/details/gqadcwtxl.sHtML

[R22] 截取子串
来源：http://3g.fanxiaobao.xyz/Article/details/gdrachawo.sHtML

echo "${s:0:5}"
来源：http://baike.fanxiaobao.xyz/Article/details/gsbglcjwj.sHtML

[R23] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghilwhzau.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggxqdbujr.sHtML

[R24] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gvhddsprs.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnpwngbi.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fanxiaobao.xyz/Article/details/gnzfgdlmb.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fanxiaobao.xyz/Article/details/ghxeamroy.sHtML

[R26] 命令替换
来源：http://3g.fanxiaobao.xyz/Article/details/gpgvzzaut.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fanxiaobao.xyz/Article/details/glyrhhuya.sHtML

[R27] 算术展开
来源：http://blog.fanxiaobao.xyz/Article/details/gjxlqejrw.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fanxiaobao.xyz/Article/details/gqehhnikr.sHtML

[R28] 浮点运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghllrsawp.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fanxiaobao.xyz/Article/details/gyttdupxe.sHtML

[R29] 定义函数
来源：http://wap.fanxiaobao.xyz/Article/details/gnznaeikt.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gtarorarm.sHtML

[R30] 函数返回状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gtvfinpmf.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtclmcfxh.sHtML

[R31] 局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gtyxfnvul.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gyamvnwmb.sHtML

[R32] 参数个数校验
来源：http://3g.fanxiaobao.xyz/Article/details/gludczsuw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/glhsfasve.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvwyikaxw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fanxiaobao.xyz/Article/details/gbkhyuwgk.sHtML

[R34] 退出时清理
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqoonczv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gqjmnthjy.sHtML

[R35] 后台执行并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/gcuzwvxnm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fanxiaobao.xyz/Article/details/gxtrbizds.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gvhkolerd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fanxiaobao.xyz/Article/details/gplljkgep.sHtML

[R37] 把输出赋给变量
来源：http://blog.fanxiaobao.xyz/Article/details/gpsxrzncm.sHtML

files=$(ls -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gprijprik.sHtML

[R38] 管道串联
来源：http://wap.fanxiaobao.xyz/Article/details/gimsamdsq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fanxiaobao.xyz/Article/details/gpdesswri.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gicumxmnt.sHtML

cmd > out.log 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjaomlqk.sHtML

[R40] 追加写日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gtlqvbdnn.sHtML

echo "log" >> out.log
来源：http://baike.fanxiaobao.xyz/Article/details/ggijvfjkf.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/grdodymkc.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gclsislhl.sHtML

[R42] 输入重定向
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghrcxfzgd.sHtML

wc -l < a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/giifyvtyg.sHtML

[R43] 按名字查找文件
来源：http://wap.fanxiaobao.xyz/Article/details/gapltddmn.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giuvaictx.sHtML

[R44] 按修改时间查找
来源：http://www.share.fanxiaobao.xyz/Article/details/ggfqfdcba.sHtML

find . -mtime -7 -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gllbnrsia.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfrvnhocc.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fanxiaobao.xyz/Article/details/gxcybzmux.sHtML

[R46] 递归替换文件内容
来源：http://blog.fanxiaobao.xyz/Article/details/gdqjtpfea.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fanxiaobao.xyz/Article/details/gzbaiwbqo.sHtML

[R47] sed 单行替换
来源：http://3g.fanxiaobao.xyz/Article/details/ghypgcyli.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gntsgcvoq.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gggltfzbi.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gdlcbdzjh.sHtML

[R49] awk 带条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjyfjhawu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fanxiaobao.xyz/Article/details/gwabzhcnl.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtednwaf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gtayhfuxc.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzcpjdnfy.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fanxiaobao.xyz/Article/details/gidmeaboy.sHtML

[R52] 统计行数
来源：http://mobile.fanxiaobao.xyz/Article/details/gvavjjiax.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gxuneauhr.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fanxiaobao.xyz/Article/details/geqsztlsi.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gfqhxbwep.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpuibebxs.sHtML

diff a.txt b.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gxopisckk.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/gtmlduhch.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fanxiaobao.xyz/Article/details/gsdnpvxfp.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gqrgfwekh.sHtML

scp file user@host:/path/
来源：http://3g.fanxiaobao.xyz/Article/details/ggnlzubbq.sHtML

[R57] 远程执行命令
来源：http://3g.fanxiaobao.xyz/Article/details/gemktdvep.sHtML

ssh user@host 'uptime'
来源：http://3g.fanxiaobao.xyz/Article/details/gfgujcquk.sHtML

[R58] 下载文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gtaxdjmhc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fanxiaobao.xyz/Article/details/geekudzlk.sHtML

[R59] 发 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gaoxpfhrx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxlxkyazg.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gywdtyayk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glxpxmcjj.sHtML

[R61] 磁盘占用
来源：http://wap.fanxiaobao.xyz/Article/details/ghhtckhql.sHtML

df -h;  du -sh *
来源：http://blog.fanxiaobao.xyz/Article/details/gyjriziqb.sHtML

[R62] 找最占空间的文件
来源：http://blog.fanxiaobao.xyz/Article/details/gxhxuqznf.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fanxiaobao.xyz/Article/details/grfvojvms.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gozgtxedj.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggobzskxg.sHtML

[R64] 结束进程
来源：http://wap.fanxiaobao.xyz/Article/details/gfuojxano.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fanxiaobao.xyz/Article/details/gpoyohoqs.sHtML

[R65] 查看端口占用
来源：http://blog.fanxiaobao.xyz/Article/details/galqwdtqk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fanxiaobao.xyz/Article/details/gktlfctaw.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gcudmcccd.sHtML

crontab -e;  crontab -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gptiyvutq.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fanxiaobao.xyz/Article/details/gkhpxfrfx.sHtML

openssl rand -hex 16
来源：http://3g.fanxiaobao.xyz/Article/details/gkqxvacvy.sHtML

[R68] 计算文件校验值
来源：http://m.share.fanxiaobao.xyz/Article/details/glnptsrbf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gnwwynqvq.sHtML

[R69] 生成随机密码
来源：http://mobile.fanxiaobao.xyz/Article/details/guttbanph.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fanxiaobao.xyz/Article/details/gblblvoje.sHtML

[R70] 时间戳与互转
来源：http://www.share.fanxiaobao.xyz/Article/details/gysaspdrj.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fanxiaobao.xyz/Article/details/gsdsrjybx.sHtML

[R71] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdyfvvtme.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fanxiaobao.xyz/Article/details/gywgjzcpc.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/gyccmbcbi.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gjjewpita.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzietsyzr.sHtML

split -l 1000 big.log part_
来源：http://blog.fanxiaobao.xyz/Article/details/gidlpvvnh.sHtML

[R74] 批量重命名
来源：http://www.share.fanxiaobao.xyz/Article/details/gfhpwbtht.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gcegxfpqu.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gsizbahno.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fanxiaobao.xyz/Article/details/guxldbpta.sHtML

[R76] 使用临时文件
来源：http://m.share.fanxiaobao.xyz/Article/details/grclpaxmg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gvbzplnjk.sHtML

[R77] 读取用户输入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtvympjxu.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/gerirngse.sHtML

[R78] 交互式菜单
来源：http://baike.fanxiaobao.xyz/Article/details/gjpbzztdy.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/gobmlfeau.sHtML

[R79] 解析命令行选项
来源：http://mobile.fanxiaobao.xyz/Article/details/gweblofdq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fanxiaobao.xyz/Article/details/gqwneoqkr.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fanxiaobao.xyz/Article/details/gnciadpmo.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbzjquam.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gnnbuvbff.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gtbximoam.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gjznqnlyu.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmveddosz.sHtML

#include <stdio.h>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guczgrfkk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbklpfaxg.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdbxfodaq.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fanxiaobao.xyz/Article/details/glfjlyxty.sHtML

[S03] C：读入整数
来源：http://baike.fanxiaobao.xyz/Article/details/giqbdvwnk.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fanxiaobao.xyz/Article/details/gltrvxkbi.sHtML

[S04] C：字符串复制
来源：http://www.blog.fanxiaobao.xyz/Article/details/grjkdfikn.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/gmmxxczkq.sHtML

[S05] C：字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqildtkhq.sHtML

strlen(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gktjzxgwe.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwrmfyzzp.sHtML

strcmp(a, b) == 0
来源：http://blog.fanxiaobao.xyz/Article/details/gtnlijpat.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/gbsgatswk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fanxiaobao.xyz/Article/details/getbfxxel.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fanxiaobao.xyz/Article/details/ghxxgjqph.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxqurjwaa.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fanxiaobao.xyz/Article/details/gjebjmboq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fanxiaobao.xyz/Article/details/guppyrody.sHtML

[S10] C：指针与解引用
来源：http://m.share.fanxiaobao.xyz/Article/details/gbqjszbga.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fanxiaobao.xyz/Article/details/gkifnutik.sHtML

[S11] C：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gdvgxtxzp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fanxiaobao.xyz/Article/details/guuiirzzv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gvweywcnk.sHtML

fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gqfacesxg.sHtML

[S12] C：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtocbggak.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gjsyaylrj.sHtML

[S13] C：宏定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gknhemgts.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fanxiaobao.xyz/Article/details/gvgfffrcy.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gaihnngfr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fanxiaobao.xyz/Article/details/gdcwoylix.sHtML

[S15] C：类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gghtuyrhn.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gdduarghq.sHtML

[S16] C：位操作置位
来源：http://baike.fanxiaobao.xyz/Article/details/ghlixshnx.sHtML

x |= (1 << 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gpwobqdkm.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzvzukbqs.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjoynnkx.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gajayzguh.sHtML

int main(int argc, char **argv)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzgsbtvdf.sHtML

[S19] C：快速排序
来源：http://baike.fanxiaobao.xyz/Article/details/gbbelzype.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxmocygud.sHtML

[S20] C：二分查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggobeesyo.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/grulgawjt.sHtML

[S21] C：字符类别判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gitczpcqj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbhfzyeze.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmqshxpk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbzyzxcfd.sHtML

[S23] C：随机数
来源：http://www.share.fanxiaobao.xyz/Article/details/ghdepkymz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmrnuvzqm.sHtML

[S24] C：获取本地时间
来源：http://blog.fanxiaobao.xyz/Article/details/giuwmkrxi.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghsmswgpe.sHtML

[S25] C：内存拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gjynukybe.sHtML

memcpy(dst, src, n);
来源：http://m.share.fanxiaobao.xyz/Article/details/gaszzcxca.sHtML

[S26] C：内存清零
来源：http://baike.fanxiaobao.xyz/Article/details/gvazdtiey.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fanxiaobao.xyz/Article/details/gsbjaziwe.sHtML

[S27] C：定义常量
来源：http://baike.fanxiaobao.xyz/Article/details/gknmsgbou.sHtML

const double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/grwajudhr.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/ggjyvvlpw.sHtML

static int counter = 0;
来源：http://blog.fanxiaobao.xyz/Article/details/gtdngoada.sHtML

[S29] C：变参函数
来源：http://blog.fanxiaobao.xyz/Article/details/gvwwhcrwz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/grcmbfagg.sHtML

[S30] C：头文件保护
来源：http://baike.fanxiaobao.xyz/Article/details/gblycvxim.sHtML

#ifndef X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gtmukdhxs.sHtML

#define X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gsoekapti.sHtML

#endif
来源：http://3g.fanxiaobao.xyz/Article/details/gkrljctog.sHtML

[S31] C++：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gxpktuhqq.sHtML

#include <iostream>
来源：http://wap.fanxiaobao.xyz/Article/details/gupfcjbys.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzyuogblp.sHtML

[S32] C++：字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmpjwoei.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fanxiaobao.xyz/Article/details/gjblvrtei.sHtML

[S33] C++：vector 增删
来源：http://wap.fanxiaobao.xyz/Article/details/gbrmnzsfa.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/giulzyjjw.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fanxiaobao.xyz/Article/details/gvouibjjn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/giigovbdc.sHtML

[S35] C++：map
来源：http://3g.fanxiaobao.xyz/Article/details/gghthujta.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gqcarrlzo.sHtML

[S36] C++：unordered_map
来源：http://3g.fanxiaobao.xyz/Article/details/gzpdcjloz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghqhncgon.sHtML

[S37] C++：set
来源：http://3g.fanxiaobao.xyz/Article/details/gpdygxrmm.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fanxiaobao.xyz/Article/details/godcilmri.sHtML

[S38] C++：排序
来源：http://baike.fanxiaobao.xyz/Article/details/gltkzyqir.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggqcwfmmd.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gpyrscixo.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fanxiaobao.xyz/Article/details/gswckuwuf.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqyesowbh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gazrreqkw.sHtML

[S41] C++：类与构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/gwgdhkgwf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fanxiaobao.xyz/Article/details/gahvdpsyi.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/grepdqcqh.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fanxiaobao.xyz/Article/details/glncoxqam.sHtML

[S43] C++：智能指针
来源：http://mobile.fanxiaobao.xyz/Article/details/gjgviigzz.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmblxztdu.sHtML

[S44] C++：引用传参
来源：http://read.share.fanxiaobao.xyz/Article/details/griblkhkb.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxponyegx.sHtML

[S45] C++：lambda
来源：http://read.share.fanxiaobao.xyz/Article/details/gembcdhcz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fanxiaobao.xyz/Article/details/gugybfrhl.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpvyinkt.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gojjrupwd.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghrpjlpna.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gayiarrdz.sHtML

[S48] C++：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gvncjqaxy.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghaxrsphn.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gedxhthsm.sHtML

[S49] C++：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/galfjelza.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fanxiaobao.xyz/Article/details/grffnznaw.sHtML

[S50] C++：格式化数字
来源：http://baike.fanxiaobao.xyz/Article/details/gnujchetj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gjtlgbpvx.sHtML

[S51] C++：显式类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gqjdmizwh.sHtML

static_cast<double>(a) / b
来源：http://baike.fanxiaobao.xyz/Article/details/gkehcanyw.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fanxiaobao.xyz/Article/details/gmqmudoem.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fanxiaobao.xyz/Article/details/gkupysfzp.sHtML

[S53] C++：移动语义
来源：http://read.share.fanxiaobao.xyz/Article/details/gmhzrarbe.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwvxqrdyw.sHtML

[S54] C++：异常处理
来源：http://blog.fanxiaobao.xyz/Article/details/gzbpjwjyf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvpzufrwo.sHtML

[S55] C++：结构化绑定
来源：http://wap.fanxiaobao.xyz/Article/details/gsmhxmboy.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghzaqknkw.sHtML

[S56] C++：optional
来源：http://blog.fanxiaobao.xyz/Article/details/gffuhbyqx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fanxiaobao.xyz/Article/details/ghavbxpem.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkkovtqjy.sHtML

constexpr int N = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcosysyno.sHtML

[S58] C++：命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/ggjfzuwon.sHtML


<!-- 参考信息 -->