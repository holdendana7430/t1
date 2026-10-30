代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpfsfrmnz.sHtML

[Q90] 生成序号列
来源：http://www.share.fanxiaobao.xyz/Article/details/ghunxavwf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fanxiaobao.xyz/Article/details/gkjnqodfz.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfycutikp.sHtML

R. Bash 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvniiqhph.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/grwltxfea.sHtML

[R01] shebang 与严格模式
来源：http://baike.fanxiaobao.xyz/Article/details/gtuxhmane.sHtML

#!/usr/bin/env bash
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwhnkipb.sHtML

set -euo pipefail
来源：http://baike.fanxiaobao.xyz/Article/details/gqzolbkke.sHtML

[R02] 变量赋值与使用
来源：http://wap.fanxiaobao.xyz/Article/details/grnmljakp.sHtML

name="Tom"; echo "$name"
来源：http://3g.fanxiaobao.xyz/Article/details/gehtrtkps.sHtML

[R03] 只读变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnfgjpxcf.sHtML

readonly PI=3.14
来源：http://www.share.fanxiaobao.xyz/Article/details/glzbdujny.sHtML

[R04] 位置参数
来源：http://baike.fanxiaobao.xyz/Article/details/gbtjvseqy.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fanxiaobao.xyz/Article/details/gujaktkjq.sHtML

[R05] 参数默认值
来源：http://3g.fanxiaobao.xyz/Article/details/grktnbnxt.sHtML

name="${1:-default}"
来源：http://wap.fanxiaobao.xyz/Article/details/gsfecgxqf.sHtML

[R06] 判断命令是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/gzbskhsnd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gbfzlymjq.sHtML

[R07] if 判断文件
来源：http://mobile.fanxiaobao.xyz/Article/details/guuqdwoeu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqrxxoviq.sHtML

[R08] 数值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gqzybpbaa.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/ghidedoew.sHtML

[R09] 字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/glrdomvlu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/ggvgumlbc.sHtML

[R10] 正则匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gidxawysc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/ghouiphtx.sHtML

[R11] case 多分支
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grwvwjmjx.sHtML

case "$1" in
来源：http://read.share.fanxiaobao.xyz/Article/details/glxfybjqx.sHtML

start) echo "启动" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gfnswfymq.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gikxpvzns.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gkyhylhjx.sHtML

esac
来源：http://m.share.fanxiaobao.xyz/Article/details/gjwkzohot.sHtML

[R12] for 遍历文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gcadykcee.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gjyirbuaq.sHtML

[R13] for 计数循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gniglgkkh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gihmijsof.sHtML

[R14] C 风格 for
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gegdycxdl.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gpfgtwxrj.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggjsctvzd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/glgnltwep.sHtML

[R16] until 等待条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gdurzkddb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gngtzkuxl.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyrdzmndz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gaybwpmzh.sHtML

[R18] 遍历数组
来源：http://wap.fanxiaobao.xyz/Article/details/gymwvaadj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjytnfso.sHtML

[R19] 数组长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggfsquzea.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjukemqrk.sHtML

[R20] 关联数组（字典）
来源：http://3g.fanxiaobao.xyz/Article/details/gqdfmlizk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gwshcabal.sHtML

[R21] 字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gasckilwb.sHtML

echo "${#s}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpbllcnfg.sHtML

[R22] 截取子串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goysfhfrm.sHtML

echo "${s:0:5}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gydkqqvzs.sHtML

[R23] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/goclsiodg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqqyzpdx.sHtML

[R24] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gqthardxf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/gwrdomsyk.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fanxiaobao.xyz/Article/details/gdbxeculv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fanxiaobao.xyz/Article/details/gyesiweia.sHtML

[R26] 命令替换
来源：http://blog.fanxiaobao.xyz/Article/details/guzvvirao.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fanxiaobao.xyz/Article/details/gghrsqhxs.sHtML

[R27] 算术展开
来源：http://mobile.fanxiaobao.xyz/Article/details/gchrrtzll.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fanxiaobao.xyz/Article/details/giibcdcnq.sHtML

[R28] 浮点运算
来源：http://read.share.fanxiaobao.xyz/Article/details/gwzdpqhfj.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fanxiaobao.xyz/Article/details/gwqtbevif.sHtML

[R29] 定义函数
来源：http://blog.fanxiaobao.xyz/Article/details/gwdshkyxr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fanxiaobao.xyz/Article/details/gfcpkvvwn.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmzcsdcw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fanxiaobao.xyz/Article/details/gfmvyengo.sHtML

[R31] 局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gubanefzt.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fanxiaobao.xyz/Article/details/guneboaso.sHtML

[R32] 参数个数校验
来源：http://3g.fanxiaobao.xyz/Article/details/gnfqhsser.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfdyaunlj.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fanxiaobao.xyz/Article/details/goiautbln.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glmgeylsk.sHtML

[R34] 退出时清理
来源：http://blog.fanxiaobao.xyz/Article/details/goshpnojx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gekjtmjfj.sHtML

[R35] 后台执行并等待
来源：http://3g.fanxiaobao.xyz/Article/details/gkncsfwvm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fanxiaobao.xyz/Article/details/gxdwxycgm.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtsghlqfc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fanxiaobao.xyz/Article/details/gqzvxoahy.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gldbvrjoy.sHtML

files=$(ls -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqwrvxrhh.sHtML

[R38] 管道串联
来源：http://read.share.fanxiaobao.xyz/Article/details/gnjuxwkro.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gevkimehf.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gldsqieli.sHtML

cmd > out.log 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gcsmzojjs.sHtML

[R40] 追加写日志
来源：http://3g.fanxiaobao.xyz/Article/details/gjoswegft.sHtML

echo "log" >> out.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gdfqfjumy.sHtML

[R41] 丢弃输出
来源：http://m.share.fanxiaobao.xyz/Article/details/ggjcjtbik.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gwbfcakrz.sHtML

[R42] 输入重定向
来源：http://baike.fanxiaobao.xyz/Article/details/giqymzrhp.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gajecspyp.sHtML

[R43] 按名字查找文件
来源：http://m.share.fanxiaobao.xyz/Article/details/glnwvebum.sHtML

find . -name "*.log" -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gngirzxqf.sHtML

[R44] 按修改时间查找
来源：http://3g.fanxiaobao.xyz/Article/details/gqcsuknbq.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxrxopzuk.sHtML

[R45] 批量删除
来源：http://wap.fanxiaobao.xyz/Article/details/guijivtzi.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fanxiaobao.xyz/Article/details/gqzdkwebg.sHtML

[R46] 递归替换文件内容
来源：http://3g.fanxiaobao.xyz/Article/details/gmjlugsmc.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fanxiaobao.xyz/Article/details/gxlzdklad.sHtML

[R47] sed 单行替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpvqbbjds.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gsdilxdlu.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/glqfhclpw.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gjqmzaxrq.sHtML

[R49] awk 带条件
来源：http://3g.fanxiaobao.xyz/Article/details/gvixkvyro.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fanxiaobao.xyz/Article/details/gvdgjlssh.sHtML

[R50] awk 求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gvhopbbub.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gpigfymkj.sHtML

[R51] 排序去重取前几
来源：http://wap.fanxiaobao.xyz/Article/details/ghqcohhin.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdkqeptpq.sHtML

[R52] 统计行数
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjpfrfbp.sHtML

wc -l a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gdlzubfrf.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fanxiaobao.xyz/Article/details/gdikiiflo.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gimuyslta.sHtML

[R54] 比较两个文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gesiwprvc.sHtML

diff a.txt b.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqychjjh.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/gkbvkqigc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/gtaabrsuy.sHtML

[R56] 远程拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gahmyftqk.sHtML

scp file user@host:/path/
来源：http://www.share.fanxiaobao.xyz/Article/details/guutxacwh.sHtML

[R57] 远程执行命令
来源：http://m.share.fanxiaobao.xyz/Article/details/ggskjwffa.sHtML

ssh user@host 'uptime'
来源：http://www.share.fanxiaobao.xyz/Article/details/gdrtbakcp.sHtML

[R58] 下载文件
来源：http://blog.fanxiaobao.xyz/Article/details/gnhqvqmhs.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fanxiaobao.xyz/Article/details/gchnanjyw.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gccgrlhwg.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fanxiaobao.xyz/Article/details/gjmuiffgp.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gngrtsuhh.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fanxiaobao.xyz/Article/details/gufejdfgt.sHtML

[R61] 磁盘占用
来源：http://3g.fanxiaobao.xyz/Article/details/gachzuwzw.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/gpkgfypft.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fanxiaobao.xyz/Article/details/ghucikiuv.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcohsmquc.sHtML

[R63] 内存与进程
来源：http://3g.fanxiaobao.xyz/Article/details/gepfosssg.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fanxiaobao.xyz/Article/details/gwoovxzbt.sHtML

[R64] 结束进程
来源：http://3g.fanxiaobao.xyz/Article/details/geenrigfq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqlwwsoyl.sHtML

[R65] 查看端口占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqstsycr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fanxiaobao.xyz/Article/details/gnszlltqg.sHtML

[R66] 定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/gxuyhrgoc.sHtML

crontab -e;  crontab -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gemteivjs.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fanxiaobao.xyz/Article/details/gcxdralxc.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/gohizgzmf.sHtML

[R68] 计算文件校验值
来源：http://wap.fanxiaobao.xyz/Article/details/gmvwzcnid.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gnmyxifwg.sHtML

[R69] 生成随机密码
来源：http://mobile.fanxiaobao.xyz/Article/details/gybhyndte.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwxaajwgb.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/ggowrxenl.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fanxiaobao.xyz/Article/details/goqxvkemx.sHtML

[R71] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gowomoyvm.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fanxiaobao.xyz/Article/details/guhzpprhj.sHtML

[R72] 等待端口就绪
来源：http://read.share.fanxiaobao.xyz/Article/details/gdamwjwzo.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gabarffjf.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndufvjks.sHtML

split -l 1000 big.log part_
来源：http://www.share.fanxiaobao.xyz/Article/details/gyzfrmzrb.sHtML

[R74] 批量重命名
来源：http://read.share.fanxiaobao.xyz/Article/details/grnswctup.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gpntecpmi.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgqxkoae.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fanxiaobao.xyz/Article/details/gzhjzusno.sHtML

[R76] 使用临时文件
来源：http://baike.fanxiaobao.xyz/Article/details/gklcpazor.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gvuhlqqop.sHtML

[R77] 读取用户输入
来源：http://wap.fanxiaobao.xyz/Article/details/guvbxuxqe.sHtML

read -rp "请输入: " ans
来源：http://read.share.fanxiaobao.xyz/Article/details/gshdfwqsd.sHtML

[R78] 交互式菜单
来源：http://read.share.fanxiaobao.xyz/Article/details/gqlicarpy.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gttuyrrkc.sHtML

[R79] 解析命令行选项
来源：http://wap.fanxiaobao.xyz/Article/details/gtogjsbfn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gvgvgurvw.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevbyirva.sHtML

time ./run.sh
来源：http://mobile.fanxiaobao.xyz/Article/details/gipsfwvib.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gbxahgoyd.sHtML

S. C / C++ 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gddwtsotk.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gyudvjtvp.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gogljaiag.sHtML

#include <stdio.h>
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggsxpngvt.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fanxiaobao.xyz/Article/details/glriyyrei.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fanxiaobao.xyz/Article/details/gmuxqoiyu.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fanxiaobao.xyz/Article/details/grhqycjoc.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gnfodcojn.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjoklwpdq.sHtML

[S04] C：字符串复制
来源：http://wap.fanxiaobao.xyz/Article/details/gititdjmp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fanxiaobao.xyz/Article/details/gmptvwdoz.sHtML

[S05] C：字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gtvqarnog.sHtML

strlen(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkvhtcmlq.sHtML

[S06] C：字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/ggycftxfo.sHtML

strcmp(a, b) == 0
来源：http://3g.fanxiaobao.xyz/Article/details/galwcwhao.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gvparkrwa.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fanxiaobao.xyz/Article/details/gckuogrym.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fanxiaobao.xyz/Article/details/gsmgjydzw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjrrskzhk.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnkfgpahe.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fanxiaobao.xyz/Article/details/gfybcrilu.sHtML

[S10] C：指针与解引用
来源：http://3g.fanxiaobao.xyz/Article/details/gfhxdaxtm.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdnjlkdoz.sHtML

[S11] C：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gvvftmqaa.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkxuhvbxm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqvzoqun.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamntynms.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gmnbgwifc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmzgvvwb.sHtML

[S13] C：宏定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gclmctexg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fanxiaobao.xyz/Article/details/glqlnkqrg.sHtML

[S14] C：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/ggdafjbop.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fanxiaobao.xyz/Article/details/gocrrpvie.sHtML

[S15] C：类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gcvgtxlwc.sHtML

(double) a / b
来源：http://wap.fanxiaobao.xyz/Article/details/gbvaupstc.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/gmbugylgk.sHtML

x |= (1 << 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkrrxkbkg.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gytqqbbmv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfhhymps.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gyecqqvxv.sHtML

int main(int argc, char **argv)
来源：http://www.share.fanxiaobao.xyz/Article/details/gczzzsoef.sHtML

[S19] C：快速排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gqoultqnw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/godnrclps.sHtML

[S20] C：二分查找
来源：http://wap.fanxiaobao.xyz/Article/details/gfjoobiwj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/guikfeacm.sHtML

[S21] C：字符类别判断
来源：http://baike.fanxiaobao.xyz/Article/details/gfftbyqvq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gorsbzeny.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/gpbmdmdvi.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggyvmaimb.sHtML

[S23] C：随机数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbiwlxzn.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzycohvjj.sHtML

[S24] C：获取本地时间
来源：http://read.share.fanxiaobao.xyz/Article/details/ghrlxgfgy.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fanxiaobao.xyz/Article/details/gzssugqvn.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gslfnwdza.sHtML

memcpy(dst, src, n);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnmjrgdlp.sHtML

[S26] C：内存清零
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guphfewfs.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzhskbrrk.sHtML

[S27] C：定义常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkryfflbi.sHtML

const double PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gyzjknbpm.sHtML

[S28] C：静态变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gutmajplp.sHtML

static int counter = 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkszgsuej.sHtML

[S29] C：变参函数
来源：http://read.share.fanxiaobao.xyz/Article/details/glunrfcqj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbnjmgvuv.sHtML

[S30] C：头文件保护
来源：http://www.share.fanxiaobao.xyz/Article/details/gidngmcgh.sHtML

#ifndef X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gryzcksul.sHtML

#define X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gwrunubbk.sHtML

#endif
来源：http://read.share.fanxiaobao.xyz/Article/details/ggxgfhcvy.sHtML

[S31] C++：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/glzokohkm.sHtML

#include <iostream>
来源：http://3g.fanxiaobao.xyz/Article/details/gccypfoxw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtlighpna.sHtML

[S32] C++：字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gampwuriz.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fanxiaobao.xyz/Article/details/gukpforps.sHtML

[S33] C++：vector 增删
来源：http://blog.fanxiaobao.xyz/Article/details/gsgzxcnnu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gnefznxkg.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fanxiaobao.xyz/Article/details/gvayunjeo.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gwmsvnzxr.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/gxkcjymcn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gucymfsfx.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gibtiktlu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsaniqxtw.sHtML

[S37] C++：set
来源：http://m.share.fanxiaobao.xyz/Article/details/gaaxcmxmq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdbziqzig.sHtML

[S38] C++：排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gzmdezrjf.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/govspwixy.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/geyqnmorv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fanxiaobao.xyz/Article/details/ggyjnhtna.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gkjmmbmvk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpgtulzzl.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnccgfjqb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gackzstbt.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fanxiaobao.xyz/Article/details/gcgtmntbw.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxknogvn.sHtML

[S43] C++：智能指针
来源：http://baike.fanxiaobao.xyz/Article/details/gohkihapj.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjxyeujpi.sHtML

[S44] C++：引用传参
来源：http://blog.fanxiaobao.xyz/Article/details/gantdlitx.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/givrkojky.sHtML

[S45] C++：lambda
来源：http://3g.fanxiaobao.xyz/Article/details/gjtzbnxpf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fanxiaobao.xyz/Article/details/grqbjwyjw.sHtML

[S46] C++：函数模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gigolawsx.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fanxiaobao.xyz/Article/details/ggrtiucxh.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzpwvfym.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gucojdcso.sHtML

[S48] C++：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gkttjbsmo.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fanxiaobao.xyz/Article/details/gqgveoeil.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glrgtnhtm.sHtML

[S49] C++：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gahrpqynw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fanxiaobao.xyz/Article/details/gmlbplwui.sHtML

[S50] C++：格式化数字
来源：http://read.share.fanxiaobao.xyz/Article/details/glwbfivqf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/geyubyahc.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzbueqxi.sHtML

static_cast<double>(a) / b
来源：http://blog.fanxiaobao.xyz/Article/details/gzxufofjx.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwrfdewxg.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmlfzdupb.sHtML

[S53] C++：移动语义
来源：http://3g.fanxiaobao.xyz/Article/details/grpmexgau.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fanxiaobao.xyz/Article/details/guirmxaqr.sHtML

[S54] C++：异常处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/getkifmbs.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/genbwwwba.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gohgoqdtb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fanxiaobao.xyz/Article/details/gtvalsuui.sHtML

[S56] C++：optional
来源：http://wap.fanxiaobao.xyz/Article/details/gigbxfksv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fanxiaobao.xyz/Article/details/guxcjzrjn.sHtML

[S57] C++：编译期常量
来源：http://m.share.fanxiaobao.xyz/Article/details/giiyaetiy.sHtML

constexpr int N = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbbwgxivi.sHtML

[S58] C++：命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/gpyfsnspz.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggdcthebc.sHtML

[S59] C++：静态断言
来源：http://baike.fanxiaobao.xyz/Article/details/gebhjrkez.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fanxiaobao.xyz/Article/details/gzpndetzo.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fanxiaobao.xyz/Article/details/gdkdvbrbx.sHtML


<!-- 参考信息 -->