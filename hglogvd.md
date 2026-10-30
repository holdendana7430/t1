代发 wailian999

name="${1:-default}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gkcfpstwy.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gztcrbqzt.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkchrisll.sHtML

[R07] if 判断文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gwuvpyope.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvuoftig.sHtML

[R08] 数值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gliuelach.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdiwthob.sHtML

[R09] 字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkrhwovg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjqqcqqd.sHtML

[R10] 正则匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gzsxjxqcf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gpceffdbj.sHtML

[R11] case 多分支
来源：http://baike.fanxiaobao.xyz/Article/details/ghqpwlbll.sHtML

case "$1" in
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggqxporxm.sHtML

start) echo "启动" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gczlwdgfp.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhfjqclu.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gemrxnslx.sHtML

esac
来源：http://mobile.fanxiaobao.xyz/Article/details/giwcqlzaa.sHtML

[R12] for 遍历文件
来源：http://blog.fanxiaobao.xyz/Article/details/gddfgmgrt.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/ghvpvuoxm.sHtML

[R13] for 计数循环
来源：http://blog.fanxiaobao.xyz/Article/details/ggcbaumdk.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gwwlqxmic.sHtML

[R14] C 风格 for
来源：http://read.share.fanxiaobao.xyz/Article/details/gxceoezbm.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gnkalqkwd.sHtML

[R15] while 逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gktlweuyk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gjupynwys.sHtML

[R16] until 等待条件
来源：http://3g.fanxiaobao.xyz/Article/details/gbrwmhoef.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/guhvugarf.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwfpjigk.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gryfjnupk.sHtML

[R18] 遍历数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gcxftzmtq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gknsttrau.sHtML

[R19] 数组长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gbufmgccx.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwdwejzki.sHtML

[R20] 关联数组（字典）
来源：http://baike.fanxiaobao.xyz/Article/details/ganwkudwr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gazgxnykt.sHtML

[R21] 字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/ghldbyhzk.sHtML

echo "${#s}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwriwzbnt.sHtML

[R22] 截取子串
来源：http://blog.fanxiaobao.xyz/Article/details/gicxpaxpi.sHtML

echo "${s:0:5}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gclhtfgrz.sHtML

[R23] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghpzsqhv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fanxiaobao.xyz/Article/details/givofwxqk.sHtML

[R24] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gpepdfodv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/gehtnfvmq.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfzlcmxy.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzivodrbm.sHtML

[R26] 命令替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gutsajlbr.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fanxiaobao.xyz/Article/details/geqwzfaio.sHtML

[R27] 算术展开
来源：http://blog.fanxiaobao.xyz/Article/details/gzrlyokkx.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvnftvexz.sHtML

[R28] 浮点运算
来源：http://mobile.fanxiaobao.xyz/Article/details/gknvavnof.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggiaoiwas.sHtML

[R29] 定义函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjfzwxdpg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gdtktgtsy.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghotwoxlt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxfxxqrq.sHtML

[R31] 局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gjahmkywv.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gkpgnbarg.sHtML

[R32] 参数个数校验
来源：http://mobile.fanxiaobao.xyz/Article/details/gqklgzqhs.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnzslzcri.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fanxiaobao.xyz/Article/details/glymzjowe.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fanxiaobao.xyz/Article/details/gzwlbbkus.sHtML

[R34] 退出时清理
来源：http://read.share.fanxiaobao.xyz/Article/details/gkihspkeo.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gixliivsb.sHtML

[R35] 后台执行并等待
来源：http://blog.fanxiaobao.xyz/Article/details/gwwfksluh.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fanxiaobao.xyz/Article/details/gaphmkuvg.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gfcizoihv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/godyddriw.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gkehrjyuo.sHtML

files=$(ls -1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzcnvibfq.sHtML

[R38] 管道串联
来源：http://3g.fanxiaobao.xyz/Article/details/gktstwlzu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhzfeddp.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fanxiaobao.xyz/Article/details/ggtywzhiq.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gqneoxjmq.sHtML

[R40] 追加写日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gyuyppgsi.sHtML

echo "log" >> out.log
来源：http://3g.fanxiaobao.xyz/Article/details/gfffmcdvh.sHtML

[R41] 丢弃输出
来源：http://wap.fanxiaobao.xyz/Article/details/gecijkrkb.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/ggbdrrejj.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/gnomodmad.sHtML

wc -l < a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/guzpnmvgd.sHtML

[R43] 按名字查找文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gmfawthef.sHtML

find . -name "*.log" -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gzmsghdxd.sHtML

[R44] 按修改时间查找
来源：http://blog.fanxiaobao.xyz/Article/details/gnugtatjt.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gwmbwcjmo.sHtML

[R45] 批量删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gsfvbvroe.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fanxiaobao.xyz/Article/details/gjktyaiyx.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fanxiaobao.xyz/Article/details/gojsmuvog.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/gjhdgpmuj.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgxvoidn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gtfvbanai.sHtML

[R48] awk 取指定列
来源：http://baike.fanxiaobao.xyz/Article/details/gjfqwabyf.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gardwcobf.sHtML

[R49] awk 带条件
来源：http://baike.fanxiaobao.xyz/Article/details/ghetflovz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fanxiaobao.xyz/Article/details/gaxrtgwge.sHtML

[R50] awk 求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gaxnsqyle.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gqftldknm.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpefxkjyl.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fanxiaobao.xyz/Article/details/gznnscijd.sHtML

[R52] 统计行数
来源：http://www.share.fanxiaobao.xyz/Article/details/gfdmyoqop.sHtML

wc -l a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/grpjvpsib.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fanxiaobao.xyz/Article/details/gqdwwgzil.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fanxiaobao.xyz/Article/details/gmnhnrndf.sHtML

[R54] 比较两个文件
来源：http://3g.fanxiaobao.xyz/Article/details/gqpiivrwq.sHtML

diff a.txt b.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gqmvpparz.sHtML

[R55] 压缩与解压
来源：http://blog.fanxiaobao.xyz/Article/details/gpogseoew.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fanxiaobao.xyz/Article/details/ghmaryypg.sHtML

[R56] 远程拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gxfmxpxcy.sHtML

scp file user@host:/path/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggnkeevzs.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/gvuswfkqy.sHtML

ssh user@host 'uptime'
来源：http://3g.fanxiaobao.xyz/Article/details/gjfqadaza.sHtML

[R58] 下载文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjqkascb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fanxiaobao.xyz/Article/details/gaowkkkpu.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/ghkdvmhta.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gfnyuesax.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/guxtlugrp.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gjobbcdxr.sHtML

[R61] 磁盘占用
来源：http://mobile.fanxiaobao.xyz/Article/details/glhrdzfwi.sHtML

df -h;  du -sh *
来源：http://blog.fanxiaobao.xyz/Article/details/giaefable.sHtML

[R62] 找最占空间的文件
来源：http://blog.fanxiaobao.xyz/Article/details/gworzxhxh.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fanxiaobao.xyz/Article/details/gurinsxwb.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gjfnbmbbg.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fanxiaobao.xyz/Article/details/gizwnkbii.sHtML

[R64] 结束进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gljxcoekw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/gcoqkfexz.sHtML

[R65] 查看端口占用
来源：http://wap.fanxiaobao.xyz/Article/details/gzjmzubkg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fanxiaobao.xyz/Article/details/gwgbxaiop.sHtML

[R66] 定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gymqxsicw.sHtML

crontab -e;  crontab -l
来源：http://baike.fanxiaobao.xyz/Article/details/grisczxfz.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fanxiaobao.xyz/Article/details/gpxkyavsi.sHtML

openssl rand -hex 16
来源：http://blog.fanxiaobao.xyz/Article/details/ganqsioeo.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdbpbzlpv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gjcjvwsxw.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsjirjijr.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fanxiaobao.xyz/Article/details/gzifxrxpv.sHtML

[R70] 时间戳与互转
来源：http://blog.fanxiaobao.xyz/Article/details/gcfoxnbyu.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/gtztlqwod.sHtML

[R71] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxcxnjooh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbcnotbce.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdymzfpnw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmaswhte.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwuasbcij.sHtML

split -l 1000 big.log part_
来源：http://wap.fanxiaobao.xyz/Article/details/gttavxjut.sHtML

[R74] 批量重命名
来源：http://baike.fanxiaobao.xyz/Article/details/gleeipovm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gufgtbmal.sHtML

[R75] 导出环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gxjebksjd.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fanxiaobao.xyz/Article/details/gowqfowfb.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdohiyzhd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gcopznwao.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcrdmyzix.sHtML

read -rp "请输入: " ans
来源：http://read.share.fanxiaobao.xyz/Article/details/gzzzseuyo.sHtML

[R78] 交互式菜单
来源：http://www.share.fanxiaobao.xyz/Article/details/gobhroufh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gjdxgnani.sHtML

[R79] 解析命令行选项
来源：http://wap.fanxiaobao.xyz/Article/details/gnpqkwasb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gztdwdakm.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/gcptkzbtv.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/giiywugih.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glgncnrdh.sHtML

S. C / C++ 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gueqniiah.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/ggkqcenrm.sHtML

[S01] C：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gzaexodfu.sHtML

#include <stdio.h>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbvifdrl.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcycwzwvk.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/gswoypqai.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fanxiaobao.xyz/Article/details/gneahxynw.sHtML

[S03] C：读入整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gexyqlcco.sHtML

int x; scanf("%d", &x);
来源：http://wap.fanxiaobao.xyz/Article/details/glqpkdxsq.sHtML

[S04] C：字符串复制
来源：http://3g.fanxiaobao.xyz/Article/details/geicjvxqg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbvdelnsq.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/ghujlyrob.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gvkzlzspm.sHtML

[S06] C：字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gidxmqmte.sHtML

strcmp(a, b) == 0
来源：http://baike.fanxiaobao.xyz/Article/details/gepqxqezl.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/ghymyouap.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fanxiaobao.xyz/Article/details/gffpovoxd.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfpllhgwf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glrpsabkz.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fanxiaobao.xyz/Article/details/gwatppker.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fanxiaobao.xyz/Article/details/gvagudwqv.sHtML

[S10] C：指针与解引用
来源：http://3g.fanxiaobao.xyz/Article/details/gmbncidcb.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gpwtfkodt.sHtML

[S11] C：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/ggcrrmrqa.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtlmgjcpv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjlnmknm.sHtML

fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gqjnbhlxa.sHtML

[S12] C：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/ggexlkhvx.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/grgnlgdkx.sHtML

[S13] C：宏定义
来源：http://wap.fanxiaobao.xyz/Article/details/gqrnhfvub.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fanxiaobao.xyz/Article/details/gzinzrfqu.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gxyxgembj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmrbfmhco.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/goohcdscp.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gpojlypkd.sHtML

[S16] C：位操作置位
来源：http://wap.fanxiaobao.xyz/Article/details/gkgphqbkh.sHtML

x |= (1 << 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqvvjlyvk.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtkawzkhc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fanxiaobao.xyz/Article/details/giabemdhx.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gwoehleax.sHtML

int main(int argc, char **argv)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbaxhuueu.sHtML

[S19] C：快速排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmjqvvyhn.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvxpckxc.sHtML

[S20] C：二分查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gagvbxxes.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpytpkgxr.sHtML

[S21] C：字符类别判断
来源：http://wap.fanxiaobao.xyz/Article/details/gbthfmzgf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guctfzehj.sHtML

[S22] C：字符串转数字
来源：http://baike.fanxiaobao.xyz/Article/details/gttrsminf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggeibmtvi.sHtML

[S23] C：随机数
来源：http://3g.fanxiaobao.xyz/Article/details/groorkmor.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fanxiaobao.xyz/Article/details/grnaaypgv.sHtML

[S24] C：获取本地时间
来源：http://blog.fanxiaobao.xyz/Article/details/gzclojtvi.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fanxiaobao.xyz/Article/details/gciuxerqv.sHtML

[S25] C：内存拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gnmjkqrmg.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gizafdcqk.sHtML

[S26] C：内存清零
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grgnyfkpa.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdthcnkbq.sHtML

[S27] C：定义常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkoqmthgx.sHtML

const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gifnlsnfh.sHtML

[S28] C：静态变量
来源：http://blog.fanxiaobao.xyz/Article/details/gzonvbuvm.sHtML

static int counter = 0;
来源：http://www.share.fanxiaobao.xyz/Article/details/gorllregq.sHtML

[S29] C：变参函数
来源：http://www.share.fanxiaobao.xyz/Article/details/guonkmikt.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fanxiaobao.xyz/Article/details/gqqepikkv.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxefjymw.sHtML

#ifndef X_H
来源：http://3g.fanxiaobao.xyz/Article/details/guaxxnruf.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gtdpxlapr.sHtML

#endif
来源：http://m.share.fanxiaobao.xyz/Article/details/gvohlshnr.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/girqnnawj.sHtML

#include <iostream>
来源：http://3g.fanxiaobao.xyz/Article/details/gsxczdktn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fanxiaobao.xyz/Article/details/geytlsgoz.sHtML

[S32] C++：字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gykzmjzjs.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fanxiaobao.xyz/Article/details/gygvdigup.sHtML

[S33] C++：vector 增删
来源：http://www.share.fanxiaobao.xyz/Article/details/gfhsnnted.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gtgisdjka.sHtML

[S34] C++：遍历 vector
来源：http://wap.fanxiaobao.xyz/Article/details/govlzziww.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gycpwsjju.sHtML

[S35] C++：map
来源：http://www.share.fanxiaobao.xyz/Article/details/gjijnoqkb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gphitpsdk.sHtML

[S36] C++：unordered_map
来源：http://3g.fanxiaobao.xyz/Article/details/glckgymfi.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/grysphqkh.sHtML

[S37] C++：set
来源：http://mobile.fanxiaobao.xyz/Article/details/gqxaaifmt.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gujtqcqzi.sHtML

[S38] C++：排序
来源：http://baike.fanxiaobao.xyz/Article/details/gexgmwvai.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gsvstrmeq.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fanxiaobao.xyz/Article/details/guofwwqah.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fanxiaobao.xyz/Article/details/genxestmr.sHtML

[S40] C++：查找元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gqtsypqzj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbrktzjto.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfzhikhrd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fanxiaobao.xyz/Article/details/gaobzvbjw.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gacvxxzve.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fanxiaobao.xyz/Article/details/gtdypqqyq.sHtML

[S43] C++：智能指针
来源：http://3g.fanxiaobao.xyz/Article/details/gknxhenkf.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fanxiaobao.xyz/Article/details/gywxqzvjm.sHtML

[S44] C++：引用传参
来源：http://m.share.fanxiaobao.xyz/Article/details/ghvkcjdbv.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwnbukeav.sHtML

[S45] C++：lambda
来源：http://baike.fanxiaobao.xyz/Article/details/gnreuidef.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gcoxswjva.sHtML

[S46] C++：函数模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gyklbkgco.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvtsrpigv.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjjesbib.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fanxiaobao.xyz/Article/details/gsnsmquki.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gwyrnfcau.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fanxiaobao.xyz/Article/details/gytbigxdj.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gdtjdcrza.sHtML

[S49] C++：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gvkaucime.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fanxiaobao.xyz/Article/details/gzogyrumv.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcqdalqaf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzahjzhvn.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gizddeqmv.sHtML

static_cast<double>(a) / b
来源：http://blog.fanxiaobao.xyz/Article/details/gqslfbaup.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fanxiaobao.xyz/Article/details/guwpdreow.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmigxqsnd.sHtML

[S53] C++：移动语义
来源：http://blog.fanxiaobao.xyz/Article/details/gsjyiozxy.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fanxiaobao.xyz/Article/details/gldtowetg.sHtML

[S54] C++：异常处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gswunwddq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gjhxaxbet.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gwhykvcuc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwacicotf.sHtML

[S56] C++：optional
来源：http://baike.fanxiaobao.xyz/Article/details/ggngiqwex.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gneewuyee.sHtML

[S57] C++：编译期常量
来源：http://mobile.fanxiaobao.xyz/Article/details/glzmfvybt.sHtML

constexpr int N = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvnxbtkdq.sHtML

[S58] C++：命名空间
来源：http://m.share.fanxiaobao.xyz/Article/details/gcmwqnksz.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfwpmbaqy.sHtML

[S59] C++：静态断言
来源：http://m.share.fanxiaobao.xyz/Article/details/gaxkzswpk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fanxiaobao.xyz/Article/details/gtenzjelp.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gdieotryq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gwoblhsny.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gdgttfieh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fanxiaobao.xyz/Article/details/gxrtpxvbs.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gsvyfeyma.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/grktnrxip.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gwdvapjki.sHtML

[T02] Kotlin：变量
来源：http://wap.fanxiaobao.xyz/Article/details/gyswemlxx.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fanxiaobao.xyz/Article/details/ghijsnifz.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fanxiaobao.xyz/Article/details/ggsazrerk.sHtML

"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/gtgvehurw.sHtML

[T04] Kotlin：空安全
来源：http://3g.fanxiaobao.xyz/Article/details/gpogammbg.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxgdorkuo.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gpfgbvgds.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxvthqqde.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fanxiaobao.xyz/Article/details/gfapyswdn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmaaakolo.sHtML


<!-- 参考信息 -->