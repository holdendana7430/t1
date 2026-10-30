代发 wailian999

readonly PI=3.14
来源：http://3g.fanxiaobao.xyz/Article/details/ggflbkytv.sHtML

[R04] 位置参数
来源：http://baike.fanxiaobao.xyz/Article/details/guehlftkw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fanxiaobao.xyz/Article/details/gctgkayql.sHtML

[R05] 参数默认值
来源：http://3g.fanxiaobao.xyz/Article/details/gpxmnyspp.sHtML

name="${1:-default}"
来源：http://3g.fanxiaobao.xyz/Article/details/gphicsqws.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhdungas.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gchvdvaps.sHtML

[R07] if 判断文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxzyukuum.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gfhwnxxcg.sHtML

[R08] 数值比较
来源：http://baike.fanxiaobao.xyz/Article/details/guegktpnc.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmkunzts.sHtML

[R09] 字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gkakplejx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmcnowpro.sHtML

[R10] 正则匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/ghcdtnzfd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gzmqebvhv.sHtML

[R11] case 多分支
来源：http://blog.fanxiaobao.xyz/Article/details/gbqljwgdz.sHtML

case "$1" in
来源：http://blog.fanxiaobao.xyz/Article/details/gyjobwctj.sHtML

start) echo "启动" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gfzhxuzdh.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjxgdyunn.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvaxmicu.sHtML

esac
来源：http://wap.fanxiaobao.xyz/Article/details/gdodyosxx.sHtML

[R12] for 遍历文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gntrwnryy.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gymfysmhk.sHtML

[R13] for 计数循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gcrhfdydr.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gexgbubbj.sHtML

[R14] C 风格 for
来源：http://m.share.fanxiaobao.xyz/Article/details/gmxbxrrqf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gjcgpczxo.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkrwcaoqj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gkhowigcn.sHtML

[R16] until 等待条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gpvtgfbni.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giuaniuii.sHtML

[R17] 数组定义与取值
来源：http://read.share.fanxiaobao.xyz/Article/details/gzvufsdob.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gkokrgbxt.sHtML

[R18] 遍历数组
来源：http://3g.fanxiaobao.xyz/Article/details/grrspsgtw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/glcgmnepe.sHtML

[R19] 数组长度
来源：http://wap.fanxiaobao.xyz/Article/details/grdasmscs.sHtML

echo "${#arr[@]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gqwsffxqr.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fanxiaobao.xyz/Article/details/gtttnytlu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfvkisfu.sHtML

[R21] 字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gjjhqlfyo.sHtML

echo "${#s}"
来源：http://read.share.fanxiaobao.xyz/Article/details/guwmlvvwr.sHtML

[R22] 截取子串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gilojkeeo.sHtML

echo "${s:0:5}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gwuxyvejq.sHtML

[R23] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/grkbvgdhw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gcpnfjxps.sHtML

[R24] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/gszgwplzq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/gtwajgeai.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fanxiaobao.xyz/Article/details/gghjlhaws.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fanxiaobao.xyz/Article/details/glsubrxfc.sHtML

[R26] 命令替换
来源：http://mobile.fanxiaobao.xyz/Article/details/ggscevglh.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvqlbylfy.sHtML

[R27] 算术展开
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsfhbdkcb.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexptxbfi.sHtML

[R28] 浮点运算
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhalxdgz.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fanxiaobao.xyz/Article/details/gxrsjvqhl.sHtML

[R29] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gqyufsadp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fanxiaobao.xyz/Article/details/ghpajahtl.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/govunafpc.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fanxiaobao.xyz/Article/details/gopuaadne.sHtML

[R31] 局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gcuueuvfi.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gysncbdwy.sHtML

[R32] 参数个数校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/grypymgbd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxufirepq.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gejasakgf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fanxiaobao.xyz/Article/details/gxnydpabx.sHtML

[R34] 退出时清理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzultvdfw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gifajhlrl.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdjcgzxgn.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fanxiaobao.xyz/Article/details/gbvxxbhhv.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkpeziny.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fanxiaobao.xyz/Article/details/gptenqbnm.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gtporqsum.sHtML

files=$(ls -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guimhiygv.sHtML

[R38] 管道串联
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvfheajjj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqsfinam.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fanxiaobao.xyz/Article/details/gukskobei.sHtML

cmd > out.log 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gxxkgzuec.sHtML

[R40] 追加写日志
来源：http://blog.fanxiaobao.xyz/Article/details/gtsudeoxx.sHtML

echo "log" >> out.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glevymhqu.sHtML

[R41] 丢弃输出
来源：http://m.share.fanxiaobao.xyz/Article/details/ggrvajtav.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwsppfxnl.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/gxzoqbirv.sHtML

wc -l < a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gyaxulcfx.sHtML

[R43] 按名字查找文件
来源：http://baike.fanxiaobao.xyz/Article/details/gnefudbbz.sHtML

find . -name "*.log" -type f
来源：http://wap.fanxiaobao.xyz/Article/details/goqewtwcb.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsocyaqzk.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmkpefmgw.sHtML

[R45] 批量删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsoqphikq.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fanxiaobao.xyz/Article/details/gfnikwdfu.sHtML

[R46] 递归替换文件内容
来源：http://baike.fanxiaobao.xyz/Article/details/gdyyyipar.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpgwxlnct.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glmomlpdv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gwmhoqjvn.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gdorcgxsh.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gmujnqczc.sHtML

[R49] awk 带条件
来源：http://blog.fanxiaobao.xyz/Article/details/gcprpfmmu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/gsggsxfsy.sHtML

[R50] awk 求和
来源：http://3g.fanxiaobao.xyz/Article/details/gklcgtowj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gasfimxei.sHtML

[R51] 排序去重取前几
来源：http://mobile.fanxiaobao.xyz/Article/details/ghjuadjot.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fanxiaobao.xyz/Article/details/gthdfozde.sHtML

[R52] 统计行数
来源：http://www.share.fanxiaobao.xyz/Article/details/gxyxjvsac.sHtML

wc -l a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/grdldefdp.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghvxzhzjr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fanxiaobao.xyz/Article/details/gopcgkvyi.sHtML

[R54] 比较两个文件
来源：http://wap.fanxiaobao.xyz/Article/details/gjmywumtl.sHtML

diff a.txt b.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gekbvqucj.sHtML

[R55] 压缩与解压
来源：http://www.blog.fanxiaobao.xyz/Article/details/geljccqlt.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fanxiaobao.xyz/Article/details/gvkrjfvzf.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gnjxwkgmv.sHtML

scp file user@host:/path/
来源：http://www.share.fanxiaobao.xyz/Article/details/gaonzjcnz.sHtML

[R57] 远程执行命令
来源：http://m.share.fanxiaobao.xyz/Article/details/gvrvheptw.sHtML

ssh user@host 'uptime'
来源：http://m.share.fanxiaobao.xyz/Article/details/ghkzfktji.sHtML

[R58] 下载文件
来源：http://3g.fanxiaobao.xyz/Article/details/gmxwygobw.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/geuflsvfz.sHtML

[R59] 发 POST JSON
来源：http://wap.fanxiaobao.xyz/Article/details/geyhunjaf.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqdhcckq.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmttoakep.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gmaazwjqw.sHtML

[R61] 磁盘占用
来源：http://mobile.fanxiaobao.xyz/Article/details/ghonrqpvl.sHtML

df -h;  du -sh *
来源：http://read.share.fanxiaobao.xyz/Article/details/grlackmka.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjsukgeb.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fanxiaobao.xyz/Article/details/gtncrhbff.sHtML

[R63] 内存与进程
来源：http://wap.fanxiaobao.xyz/Article/details/gkcxzyyvo.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fanxiaobao.xyz/Article/details/galnyjqcv.sHtML

[R64] 结束进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gtbxilvnv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfihymbgy.sHtML

[R65] 查看端口占用
来源：http://wap.fanxiaobao.xyz/Article/details/gsjhpmyqb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fanxiaobao.xyz/Article/details/gdihiuzik.sHtML

[R66] 定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/gslwbngsx.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyrhowiqd.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fanxiaobao.xyz/Article/details/gppzowdyw.sHtML

openssl rand -hex 16
来源：http://baike.fanxiaobao.xyz/Article/details/gdkikfcmn.sHtML

[R68] 计算文件校验值
来源：http://baike.fanxiaobao.xyz/Article/details/gjxlzektg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gxdernqbt.sHtML

[R69] 生成随机密码
来源：http://read.share.fanxiaobao.xyz/Article/details/gwzkpxglc.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fanxiaobao.xyz/Article/details/geullukov.sHtML

[R70] 时间戳与互转
来源：http://www.share.fanxiaobao.xyz/Article/details/gfwjmcgwm.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fanxiaobao.xyz/Article/details/gcpppxkqi.sHtML

[R71] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gavfqyqwi.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmjzjyauy.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/gjvdzqlbt.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gnaqfzxes.sHtML

[R73] 分割大日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkgibxxrd.sHtML

split -l 1000 big.log part_
来源：http://3g.fanxiaobao.xyz/Article/details/ghjedfkmf.sHtML

[R74] 批量重命名
来源：http://www.share.fanxiaobao.xyz/Article/details/gsptptzya.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gfgxhwnzm.sHtML

[R75] 导出环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/gizwogsfn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjncacpmj.sHtML

[R76] 使用临时文件
来源：http://wap.fanxiaobao.xyz/Article/details/gnfarrzns.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gsxcpzmjv.sHtML

[R77] 读取用户输入
来源：http://m.share.fanxiaobao.xyz/Article/details/gdartuauz.sHtML

read -rp "请输入: " ans
来源：http://www.share.fanxiaobao.xyz/Article/details/gcebvtisy.sHtML

[R78] 交互式菜单
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmxjwpqxk.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/gjuccolej.sHtML

[R79] 解析命令行选项
来源：http://m.share.fanxiaobao.xyz/Article/details/gxaniiiev.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfhnpapy.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fanxiaobao.xyz/Article/details/gbynginjc.sHtML

time ./run.sh
来源：http://m.share.fanxiaobao.xyz/Article/details/gdmzdhzwi.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdjynlzba.sHtML

S. C / C++ 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/genotbaec.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqeopghl.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gukkujqcf.sHtML

#include <stdio.h>
来源：http://wap.fanxiaobao.xyz/Article/details/gizldsagh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fanxiaobao.xyz/Article/details/glwqeolvs.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/gxjmuzwsg.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdnemuozy.sHtML

[S03] C：读入整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkhbxdshg.sHtML

int x; scanf("%d", &x);
来源：http://baike.fanxiaobao.xyz/Article/details/guibuatow.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/gabygorkf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fanxiaobao.xyz/Article/details/gcffvhkcg.sHtML

[S05] C：字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/grpdyxrjo.sHtML

strlen(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gdyjrasjz.sHtML

[S06] C：字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gzkpbjsjg.sHtML

strcmp(a, b) == 0
来源：http://baike.fanxiaobao.xyz/Article/details/ghgbttzzc.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghwnmmxnd.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gacteujlb.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fanxiaobao.xyz/Article/details/gyhygporm.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbatflhlr.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fanxiaobao.xyz/Article/details/glidsxjrm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/gwjbpccfc.sHtML

[S10] C：指针与解引用
来源：http://baike.fanxiaobao.xyz/Article/details/ggvffpado.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzvfrryd.sHtML

[S11] C：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gdwnwwrtu.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gczhpaxrz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gxblkeizq.sHtML

fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvstiyiks.sHtML

[S12] C：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/guudbfeph.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqdreaisa.sHtML

[S13] C：宏定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gghcdsdef.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fanxiaobao.xyz/Article/details/gpehualfa.sHtML

[S14] C：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gvlbkiqum.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzuhtzmva.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gifmpamrs.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/gbupbkrsj.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/gaguxqilp.sHtML

x |= (1 << 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gpdkgzuyi.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/glviurubt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fanxiaobao.xyz/Article/details/gcxmcraxf.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfryqiomt.sHtML

int main(int argc, char **argv)
来源：http://3g.fanxiaobao.xyz/Article/details/gnwmlijuc.sHtML

[S19] C：快速排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gfnecxmxx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gntazbcbj.sHtML

[S20] C：二分查找
来源：http://3g.fanxiaobao.xyz/Article/details/gmeyatwpr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gufuaiqwe.sHtML

[S21] C：字符类别判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gefxjidnr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzwgfoju.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/gowmxsyyj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fanxiaobao.xyz/Article/details/gqqayhupu.sHtML

[S23] C：随机数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwiugniof.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzwpaoipe.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/gmhbmoexl.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggbsszhnf.sHtML

[S25] C：内存拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gnmsvyfsp.sHtML

memcpy(dst, src, n);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkddmsyrr.sHtML

[S26] C：内存清零
来源：http://www.share.fanxiaobao.xyz/Article/details/ghezexdxc.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fanxiaobao.xyz/Article/details/guwrzksgc.sHtML

[S27] C：定义常量
来源：http://wap.fanxiaobao.xyz/Article/details/gxsaxmgjc.sHtML

const double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gaktojmln.sHtML

[S28] C：静态变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gskswyxqh.sHtML

static int counter = 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfqpbphpi.sHtML

[S29] C：变参函数
来源：http://wap.fanxiaobao.xyz/Article/details/gqlgitmaf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fanxiaobao.xyz/Article/details/guisrkptg.sHtML

[S30] C：头文件保护
来源：http://wap.fanxiaobao.xyz/Article/details/gftsfcbkj.sHtML

#ifndef X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvxsfdov.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gkaokgpfr.sHtML

#endif
来源：http://read.share.fanxiaobao.xyz/Article/details/gvqodhtkf.sHtML

[S31] C++：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gnlakpmdy.sHtML

#include <iostream>
来源：http://blog.fanxiaobao.xyz/Article/details/gyhpucwqk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdbgovgtd.sHtML

[S32] C++：字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggdwskqoh.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkmdbakg.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtdrxufpn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guwydbjzo.sHtML

[S34] C++：遍历 vector
来源：http://blog.fanxiaobao.xyz/Article/details/gylgjkoch.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goqhhiluo.sHtML

[S35] C++：map
来源：http://www.blog.fanxiaobao.xyz/Article/details/grzlvjifn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbxeiqsl.sHtML

[S36] C++：unordered_map
来源：http://wap.fanxiaobao.xyz/Article/details/gcfheqarg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/genopvaqa.sHtML

[S37] C++：set
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzbfkmacc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gihfmnkqz.sHtML

[S38] C++：排序
来源：http://blog.fanxiaobao.xyz/Article/details/gdqujjnac.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonmusquk.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fanxiaobao.xyz/Article/details/ginfyrsww.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fanxiaobao.xyz/Article/details/gvigrkybn.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gdgwttqbe.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpvjfckjy.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gnrlyswdt.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwxraaqm.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxsfcdgp.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbfwecfgs.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghpgmhlsr.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gazydxguo.sHtML

[S44] C++：引用传参
来源：http://mobile.fanxiaobao.xyz/Article/details/grmiyndul.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpfescteg.sHtML

[S45] C++：lambda
来源：http://m.share.fanxiaobao.xyz/Article/details/gkdscycpp.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gzfwpszfb.sHtML

[S46] C++：函数模板
来源：http://www.share.fanxiaobao.xyz/Article/details/goyaxfjmj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkeiowdyj.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gbcmaisws.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fanxiaobao.xyz/Article/details/glrjmwkxb.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmbfbbbs.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fanxiaobao.xyz/Article/details/gotnkpope.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqatjjlsi.sHtML

[S49] C++：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gyofpgxir.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gjpgkqrpm.sHtML

[S50] C++：格式化数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gvvurbzha.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gnnabhbwz.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gebpodmbr.sHtML

static_cast<double>(a) / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gigqyyhhc.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fanxiaobao.xyz/Article/details/geedkhnel.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fanxiaobao.xyz/Article/details/gpjgldiex.sHtML

[S53] C++：移动语义
来源：http://baike.fanxiaobao.xyz/Article/details/gbvkuskuu.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmzjpsjgc.sHtML

[S54] C++：异常处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gnzbcdpyr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/guoxtshba.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gnadgaayn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gmlosrtsk.sHtML

[S56] C++：optional
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhildnlm.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fanxiaobao.xyz/Article/details/ggxrfcbnr.sHtML

[S57] C++：编译期常量
来源：http://mobile.fanxiaobao.xyz/Article/details/glmggqchn.sHtML

constexpr int N = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gdkgwjxbh.sHtML

[S58] C++：命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/gzidiasaq.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gygnpokgp.sHtML

[S59] C++：静态断言
来源：http://baike.fanxiaobao.xyz/Article/details/gkeozhcqn.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fanxiaobao.xyz/Article/details/gnrhyyqys.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gggfyhhrs.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gqirhesse.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmftxyjo.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fanxiaobao.xyz/Article/details/gargzmrpu.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gzrflhxmb.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxufncpnk.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gpoirxclf.sHtML

[T02] Kotlin：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gnhmijpln.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdfieqek.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gemjpqzbs.sHtML

"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/gygeyxnpb.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxqumedzb.sHtML

val n: String? = null;  n?.length
来源：http://3g.fanxiaobao.xyz/Article/details/ganfpxebs.sHtML


<!-- 参考信息 -->