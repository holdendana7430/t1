代发 wailian999

set -euo pipefail
来源：http://mobile.fanxiaobao.xyz/Article/details/gugytcrun.sHtML

[R02] 变量赋值与使用
来源：http://wap.fanxiaobao.xyz/Article/details/gylijefol.sHtML

name="Tom"; echo "$name"
来源：http://3g.fanxiaobao.xyz/Article/details/ggqoqalqi.sHtML

[R03] 只读变量
来源：http://wap.fanxiaobao.xyz/Article/details/gdnohwhpi.sHtML

readonly PI=3.14
来源：http://read.share.fanxiaobao.xyz/Article/details/gwzsibqtd.sHtML

[R04] 位置参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gailkzprr.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fanxiaobao.xyz/Article/details/gajfnpqle.sHtML

[R05] 参数默认值
来源：http://3g.fanxiaobao.xyz/Article/details/gkffoiuxg.sHtML

name="${1:-default}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gvoclfdar.sHtML

[R06] 判断命令是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gzmjxyclm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gcbjwpxwd.sHtML

[R07] if 判断文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gktcicxzn.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gxuzjibxd.sHtML

[R08] 数值比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfkjolrz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvdhvxhjb.sHtML

[R09] 字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gxyistbmj.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/ghwhrjgnd.sHtML

[R10] 正则匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gepfqzhtp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/grsuvewng.sHtML

[R11] case 多分支
来源：http://www.share.fanxiaobao.xyz/Article/details/gkncfyyks.sHtML

case "$1" in
来源：http://m.share.fanxiaobao.xyz/Article/details/gbhwolcpy.sHtML

start) echo "启动" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbqbaalh.sHtML

stop)  echo "停止" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gpgnaqbmy.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/guapsvfjo.sHtML

esac
来源：http://m.share.fanxiaobao.xyz/Article/details/geeyebntj.sHtML

[R12] for 遍历文件
来源：http://3g.fanxiaobao.xyz/Article/details/gxrsehouw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gsxhefuqg.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gpufhzrvo.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gnnrljumb.sHtML

[R14] C 风格 for
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbuujwsv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/giyuecsss.sHtML

[R15] while 逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gfvtjfoqz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gfxliwedo.sHtML

[R16] until 等待条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjpubnkwx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gvlytmwvd.sHtML

[R17] 数组定义与取值
来源：http://wap.fanxiaobao.xyz/Article/details/gdipawsgb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gfwixriae.sHtML

[R18] 遍历数组
来源：http://read.share.fanxiaobao.xyz/Article/details/gxgtpppyg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fanxiaobao.xyz/Article/details/ggdhublsx.sHtML

[R19] 数组长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gsuokqfuc.sHtML

echo "${#arr[@]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gsunectir.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhrpimhk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gphmgbrxj.sHtML

[R21] 字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/ggzbrosyc.sHtML

echo "${#s}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grmaatxgk.sHtML

[R22] 截取子串
来源：http://www.share.fanxiaobao.xyz/Article/details/grhxmxiof.sHtML

echo "${s:0:5}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/glthcoccz.sHtML

[R23] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gtojuvxrs.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbikyvyi.sHtML

[R24] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gybjpzgep.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbwasixkc.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzwyevht.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fanxiaobao.xyz/Article/details/gyzusxkgf.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gijrkkfnl.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fanxiaobao.xyz/Article/details/gjquzzdwx.sHtML

[R27] 算术展开
来源：http://read.share.fanxiaobao.xyz/Article/details/grvdeptxb.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fanxiaobao.xyz/Article/details/ggggyjkfr.sHtML

[R28] 浮点运算
来源：http://blog.fanxiaobao.xyz/Article/details/glxydcaag.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fanxiaobao.xyz/Article/details/gxsxycltk.sHtML

[R29] 定义函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gulbotnqz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/gfkwgrsrz.sHtML

[R30] 函数返回状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gdqltfogv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fanxiaobao.xyz/Article/details/gtpforabj.sHtML

[R31] 局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gskmlccxy.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjudhijrb.sHtML

[R32] 参数个数校验
来源：http://www.share.fanxiaobao.xyz/Article/details/gjqiqtkue.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcdbrpryz.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/glathtoph.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fanxiaobao.xyz/Article/details/gyrbtscdh.sHtML

[R34] 退出时清理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjyioigmp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gikfyshdd.sHtML

[R35] 后台执行并等待
来源：http://blog.fanxiaobao.xyz/Article/details/gtjjstvdz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdwuwycj.sHtML

[R36] 并发执行多个任务
来源：http://3g.fanxiaobao.xyz/Article/details/gzpupnadt.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fanxiaobao.xyz/Article/details/gwqwgexdj.sHtML

[R37] 把输出赋给变量
来源：http://baike.fanxiaobao.xyz/Article/details/ggzlkzqvv.sHtML

files=$(ls -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjhnwoghc.sHtML

[R38] 管道串联
来源：http://blog.fanxiaobao.xyz/Article/details/gjjcuaflj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fanxiaobao.xyz/Article/details/ggkquvmfd.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbokiqykh.sHtML

cmd > out.log 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gqrnclovp.sHtML

[R40] 追加写日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gdgroilgo.sHtML

echo "log" >> out.log
来源：http://m.share.fanxiaobao.xyz/Article/details/ggchldpbr.sHtML

[R41] 丢弃输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gpuloqwde.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gioyseeii.sHtML

[R42] 输入重定向
来源：http://m.share.fanxiaobao.xyz/Article/details/gfcyrqsar.sHtML

wc -l < a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gbhflfhig.sHtML

[R43] 按名字查找文件
来源：http://baike.fanxiaobao.xyz/Article/details/ggnrfmald.sHtML

find . -name "*.log" -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gnlncocwk.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxrmislhl.sHtML

find . -mtime -7 -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gfwzyldhb.sHtML

[R45] 批量删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcehoxfvb.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fanxiaobao.xyz/Article/details/gdseislcw.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyssgokdc.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxhcyzbtz.sHtML

[R47] sed 单行替换
来源：http://baike.fanxiaobao.xyz/Article/details/gsfpuvjru.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gtxbluyxk.sHtML

[R48] awk 取指定列
来源：http://baike.fanxiaobao.xyz/Article/details/gxixpuzzo.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gcpdlgfom.sHtML

[R49] awk 带条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwixwmomy.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/gqyfjnmdv.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/glaoulaur.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gtajmxcoz.sHtML

[R51] 排序去重取前几
来源：http://baike.fanxiaobao.xyz/Article/details/gycqjfvha.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdbvaobzz.sHtML

[R52] 统计行数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsufntqpy.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gbnuywqyb.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fanxiaobao.xyz/Article/details/gldpiavky.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjmbwjasw.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gagxkjxeb.sHtML

diff a.txt b.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gaqqoojvn.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/gbvemposf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/gnhizwmou.sHtML

[R56] 远程拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gzsybqvrs.sHtML

scp file user@host:/path/
来源：http://www.share.fanxiaobao.xyz/Article/details/gyhhvmkep.sHtML

[R57] 远程执行命令
来源：http://read.share.fanxiaobao.xyz/Article/details/gsbtslkml.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gykwjdrps.sHtML

[R58] 下载文件
来源：http://wap.fanxiaobao.xyz/Article/details/gblhdwley.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fanxiaobao.xyz/Article/details/gjbxzwaia.sHtML

[R59] 发 POST JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/glfcpuhzu.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbhrekyp.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gzppbwgjf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwwwdlfd.sHtML

[R61] 磁盘占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gzgiftxfx.sHtML

df -h;  du -sh *
来源：http://3g.fanxiaobao.xyz/Article/details/gdyahexnf.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwrsmevy.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fanxiaobao.xyz/Article/details/gzzgdovvf.sHtML

[R63] 内存与进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gceuowgkw.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fanxiaobao.xyz/Article/details/gypuaokwf.sHtML

[R64] 结束进程
来源：http://baike.fanxiaobao.xyz/Article/details/gpirolayd.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fanxiaobao.xyz/Article/details/ganjnwbek.sHtML

[R65] 查看端口占用
来源：http://baike.fanxiaobao.xyz/Article/details/gqbbwfkgx.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdwckerw.sHtML

[R66] 定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goczphrhi.sHtML

crontab -e;  crontab -l
来源：http://wap.fanxiaobao.xyz/Article/details/giptfetoo.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkazoiynl.sHtML

openssl rand -hex 16
来源：http://mobile.fanxiaobao.xyz/Article/details/grecvikcj.sHtML

[R68] 计算文件校验值
来源：http://www.share.fanxiaobao.xyz/Article/details/gbudxqugr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gcinkjloz.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghxnypcp.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gccwgifku.sHtML

[R70] 时间戳与互转
来源：http://read.share.fanxiaobao.xyz/Article/details/gajjvyico.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fanxiaobao.xyz/Article/details/gzacfxqxf.sHtML

[R71] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gidgebrcq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fanxiaobao.xyz/Article/details/glflarpix.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/gwyphvonf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/ghgocajfo.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gorskxhyf.sHtML

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/gowedyxpc.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/gxduqgmak.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gtycrauzr.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gewzavmfk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fanxiaobao.xyz/Article/details/gkmobscoy.sHtML

[R76] 使用临时文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghstovmpt.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gstikbdhm.sHtML

[R77] 读取用户输入
来源：http://wap.fanxiaobao.xyz/Article/details/gqwupneav.sHtML

read -rp "请输入: " ans
来源：http://mobile.fanxiaobao.xyz/Article/details/gzmodagqv.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/glcielrqd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjgbawlr.sHtML

[R79] 解析命令行选项
来源：http://baike.fanxiaobao.xyz/Article/details/gafujdpet.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fanxiaobao.xyz/Article/details/gvdedlyth.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdyjersyu.sHtML

time ./run.sh
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvcgholm.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gdbutztfu.sHtML

S. C / C++ 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gyznnqfsx.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gjdzgwqne.sHtML

[S01] C：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gspbpmryt.sHtML

#include <stdio.h>
来源：http://3g.fanxiaobao.xyz/Article/details/gryhttuib.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtofcskve.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggnsddpoo.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwncpjyoo.sHtML

[S03] C：读入整数
来源：http://blog.fanxiaobao.xyz/Article/details/glwxggcfs.sHtML

int x; scanf("%d", &x);
来源：http://wap.fanxiaobao.xyz/Article/details/gphyomfcz.sHtML

[S04] C：字符串复制
来源：http://3g.fanxiaobao.xyz/Article/details/gkkcqzret.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/gkabcneae.sHtML

[S05] C：字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/ghplozzxj.sHtML

strlen(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gkrqvicme.sHtML

[S06] C：字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gedemabok.sHtML

strcmp(a, b) == 0
来源：http://mobile.fanxiaobao.xyz/Article/details/gsmvzdaoz.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gqruywfix.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fanxiaobao.xyz/Article/details/garwquias.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fanxiaobao.xyz/Article/details/gujueefte.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fanxiaobao.xyz/Article/details/gzqtaohjv.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fanxiaobao.xyz/Article/details/gejtiqdfh.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fanxiaobao.xyz/Article/details/gvkhxletf.sHtML

[S10] C：指针与解引用
来源：http://read.share.fanxiaobao.xyz/Article/details/gtyfmdyjc.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxbcwipv.sHtML

[S11] C：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gdrdchdeo.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefzvlpbq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gmranqrxe.sHtML

fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gizciuxca.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gtlkosvun.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gvntzjxcp.sHtML

[S13] C：宏定义
来源：http://mobile.fanxiaobao.xyz/Article/details/ggdxmenkm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fanxiaobao.xyz/Article/details/gisxdyydl.sHtML

[S14] C：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gaqbnllul.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fanxiaobao.xyz/Article/details/gzklzgpfn.sHtML

[S15] C：类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gujknpzkf.sHtML

(double) a / b
来源：http://wap.fanxiaobao.xyz/Article/details/gwngtmvho.sHtML

[S16] C：位操作置位
来源：http://3g.fanxiaobao.xyz/Article/details/gwgfrdooq.sHtML

x |= (1 << 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gitpbvlqr.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gffraqmuv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxnxcdmmc.sHtML

[S18] C：命令行参数
来源：http://wap.fanxiaobao.xyz/Article/details/gvcwrsbcd.sHtML

int main(int argc, char **argv)
来源：http://blog.fanxiaobao.xyz/Article/details/gzofnywoq.sHtML

[S19] C：快速排序
来源：http://baike.fanxiaobao.xyz/Article/details/gfbmzwijt.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkatflnuo.sHtML

[S20] C：二分查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwowtvelu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gsttgnsod.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gimufccut.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fanxiaobao.xyz/Article/details/gtvqeylzt.sHtML

[S22] C：字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gioqmoihw.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqbjfqkbz.sHtML

[S23] C：随机数
来源：http://blog.fanxiaobao.xyz/Article/details/gzitnznpi.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gdktfaktt.sHtML

[S24] C：获取本地时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhgubvup.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfatwxnbq.sHtML

[S25] C：内存拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gocoomdie.sHtML

memcpy(dst, src, n);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpauluqau.sHtML

[S26] C：内存清零
来源：http://blog.fanxiaobao.xyz/Article/details/gamssbrwb.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxupgimvm.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/gycspcqcn.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvpkxgigo.sHtML

[S28] C：静态变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gsyxsnity.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghsdmerad.sHtML

[S29] C：变参函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gxgxplelx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjikasxy.sHtML

[S30] C：头文件保护
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqqlpaswb.sHtML

#ifndef X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gschqedcf.sHtML

#define X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/grqbctpdy.sHtML

#endif
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdgzhoko.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpltdowwv.sHtML

#include <iostream>
来源：http://m.share.fanxiaobao.xyz/Article/details/gkordsnae.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gptkjlynq.sHtML

[S32] C++：字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/glhrnfskh.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fanxiaobao.xyz/Article/details/gwhufcnmx.sHtML

[S33] C++：vector 增删
来源：http://blog.fanxiaobao.xyz/Article/details/gcmaaynxk.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvnstczcg.sHtML

[S34] C++：遍历 vector
来源：http://blog.fanxiaobao.xyz/Article/details/gwtfxlcos.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gotywdtyh.sHtML

[S35] C++：map
来源：http://www.share.fanxiaobao.xyz/Article/details/gdrqlarjr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/glhelvjli.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvnvyojbh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gliidjyci.sHtML

[S37] C++：set
来源：http://wap.fanxiaobao.xyz/Article/details/gvukjqtic.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gswjkcngd.sHtML

[S38] C++：排序
来源：http://blog.fanxiaobao.xyz/Article/details/gstwatwxe.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdkvqpszq.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gziouuwoe.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fanxiaobao.xyz/Article/details/gukfqhoov.sHtML

[S40] C++：查找元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gesnvmkdh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvwqcyhnh.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqmliypb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fanxiaobao.xyz/Article/details/gxltpqmyx.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjkfqsox.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fanxiaobao.xyz/Article/details/guinrzyra.sHtML

[S43] C++：智能指针
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxyqmexf.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fanxiaobao.xyz/Article/details/gcqgpanrx.sHtML

[S44] C++：引用传参
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhwcugfo.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqavqbdt.sHtML

[S45] C++：lambda
来源：http://wap.fanxiaobao.xyz/Article/details/gpbpjuarm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbteryklp.sHtML

[S46] C++：函数模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatdjbymw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gebeowarr.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gmgjngjpl.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gekbfipaw.sHtML

[S48] C++：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/ganxdtcon.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fanxiaobao.xyz/Article/details/gwhhbqjjh.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmwvltffc.sHtML

[S49] C++：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gnieatsla.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/gfidrgbiz.sHtML

[S50] C++：格式化数字
来源：http://3g.fanxiaobao.xyz/Article/details/ggshdzkcx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtqeucdve.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/ggsyjchum.sHtML

static_cast<double>(a) / b
来源：http://3g.fanxiaobao.xyz/Article/details/gghzqmpxj.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fanxiaobao.xyz/Article/details/glnndcigh.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fanxiaobao.xyz/Article/details/gcppuyrdz.sHtML

[S53] C++：移动语义
来源：http://3g.fanxiaobao.xyz/Article/details/grerkdmux.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdscqsvsh.sHtML

[S54] C++：异常处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gklwxpzff.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gktxkzfnf.sHtML

[S55] C++：结构化绑定
来源：http://baike.fanxiaobao.xyz/Article/details/goocpiqnc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/gppagwzhx.sHtML

[S56] C++：optional
来源：http://baike.fanxiaobao.xyz/Article/details/gbngcntfy.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fanxiaobao.xyz/Article/details/gmbqmuxql.sHtML

[S57] C++：编译期常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gtotebspx.sHtML

constexpr int N = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gujftadrl.sHtML

[S58] C++：命名空间
来源：http://wap.fanxiaobao.xyz/Article/details/gklspxkvk.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fanxiaobao.xyz/Article/details/genxsbfyw.sHtML

[S59] C++：静态断言
来源：http://www.blog.fanxiaobao.xyz/Article/details/grvliaqve.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fanxiaobao.xyz/Article/details/gshagvmuh.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fanxiaobao.xyz/Article/details/gvbjdncna.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gpfwjrkmq.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gsbmtqkdu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fanxiaobao.xyz/Article/details/gawdbmnsr.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/guwtspfro.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gtypkbjoz.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gkkamcwhb.sHtML

[T02] Kotlin：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gohhteazo.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjasgswo.sHtML


<!-- 参考信息 -->