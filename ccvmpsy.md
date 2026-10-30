代发 wailian999

set -euo pipefail
来源：http://www.blog.fehbvm.com/Article/details/gbyatbdrx.sHtML

[R02] 变量赋值与使用
来源：http://m.share.zdbjq.cn/Article/details/gvqsiybjm.sHtML

name="Tom"; echo "$name"
来源：http://baike.hesvh.cn/Article/details/gsonxlifw.sHtML

[R03] 只读变量
来源：http://wap.hesvh.cn/Article/details/gbiqomcok.sHtML

readonly PI=3.14
来源：http://www.blog.zdbjq.cn/Article/details/gpybssftw.sHtML

[R04] 位置参数
来源：http://mobile.fehbvm.com/Article/details/gasxntzzi.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.zdbjq.cn/Article/details/gktokmfoy.sHtML

[R05] 参数默认值
来源：http://www.blog.hesvh.cn/Article/details/gqndaqfto.sHtML

name="${1:-default}"
来源：http://www.m.share.fehbvm.com/Article/details/gvshbvnzj.sHtML

[R06] 判断命令是否存在
来源：http://blog.hesvh.cn/Article/details/gubdzspfd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/gwngxugcn.sHtML

[R07] if 判断文件
来源：http://m.share.fehbvm.com/Article/details/gpvzdsfzu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.hesvh.cn/Article/details/gmdkgzaws.sHtML

[R08] 数值比较
来源：http://blog.hesvh.cn/Article/details/gqmcrgshv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.zdbjq.cn/Article/details/ggadvoivf.sHtML

[R09] 字符串比较
来源：http://blog.hesvh.cn/Article/details/gbtlcivos.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fehbvm.com/Article/details/gehbhyojn.sHtML

[R10] 正则匹配
来源：http://blog.fehbvm.com/Article/details/ghkabhbgd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.hesvh.cn/Article/details/gnxftvakt.sHtML

[R11] case 多分支
来源：http://wap.fehbvm.com/Article/details/gdbxqlyvl.sHtML

case "$1" in
来源：http://3g.hesvh.cn/Article/details/gsoctwrfn.sHtML

start) echo "启动" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gfskbhecw.sHtML

stop)  echo "停止" ;;
来源：http://baike.zdbjq.cn/Article/details/gunnyhswn.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fehbvm.com/Article/details/gvwosewxn.sHtML

esac
来源：http://www.share.hesvh.cn/Article/details/gyleolxub.sHtML

[R12] for 遍历文件
来源：http://www.share.fehbvm.com/Article/details/gcdcgsdqg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fehbvm.com/Article/details/glkmwiedc.sHtML

[R13] for 计数循环
来源：http://mobile.zdbjq.cn/Article/details/gopkoswii.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fehbvm.com/Article/details/ggcrnpazi.sHtML

[R14] C 风格 for
来源：http://www.share.hesvh.cn/Article/details/gpwrbvnhs.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/gqijrbfpt.sHtML

[R15] while 逐行读文件
来源：http://wap.hesvh.cn/Article/details/glmmcrgnq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fehbvm.com/Article/details/gqgcidqoq.sHtML

[R16] until 等待条件
来源：http://m.share.fehbvm.com/Article/details/gtmoduvrm.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gwxpxzkar.sHtML

[R17] 数组定义与取值
来源：http://m.share.hesvh.cn/Article/details/gsrrralle.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.zdbjq.cn/Article/details/gfcsvjclb.sHtML

[R18] 遍历数组
来源：http://baike.zdbjq.cn/Article/details/gyvzlqasl.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fehbvm.com/Article/details/gtdohkonm.sHtML

[R19] 数组长度
来源：http://www.share.fehbvm.com/Article/details/gvimfydnd.sHtML

echo "${#arr[@]}"
来源：http://3g.fehbvm.com/Article/details/gziqtjkob.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.zdbjq.cn/Article/details/ghvqavhbu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.hesvh.cn/Article/details/gcvsgvkti.sHtML

[R21] 字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gfdjarpaf.sHtML

echo "${#s}"
来源：http://www.m.share.fehbvm.com/Article/details/govcwcdmq.sHtML

[R22] 截取子串
来源：http://baike.zdbjq.cn/Article/details/grxkymqze.sHtML

echo "${s:0:5}"
来源：http://www.share.zdbjq.cn/Article/details/gdudaudyp.sHtML

[R23] 字符串替换
来源：http://baike.hesvh.cn/Article/details/grzgzihrc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fehbvm.com/Article/details/ghtqhhtvf.sHtML

[R24] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/gnspvblnp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.zdbjq.cn/Article/details/gapyaxbmd.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.hesvh.cn/Article/details/gjvyahcdt.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.hesvh.cn/Article/details/gpuspvgpw.sHtML

[R26] 命令替换
来源：http://read.share.zdbjq.cn/Article/details/gkvlywwif.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.hesvh.cn/Article/details/glowltdye.sHtML

[R27] 算术展开
来源：http://www.m.share.hesvh.cn/Article/details/gxsdpjaaz.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fehbvm.com/Article/details/gfymjzrts.sHtML

[R28] 浮点运算
来源：http://www.blog.fehbvm.com/Article/details/geogjgsxe.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.zdbjq.cn/Article/details/gdsprirag.sHtML

[R29] 定义函数
来源：http://mobile.hesvh.cn/Article/details/glazzsuxn.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.zdbjq.cn/Article/details/gegfmjrfw.sHtML

[R30] 函数返回状态码
来源：http://baike.fehbvm.com/Article/details/gqzrpkyus.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.hesvh.cn/Article/details/ghhaudhhn.sHtML

[R31] 局部变量
来源：http://read.share.hesvh.cn/Article/details/gvbozxhlx.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fehbvm.com/Article/details/gvqfqdbkw.sHtML

[R32] 参数个数校验
来源：http://mobile.fehbvm.com/Article/details/gsprnmwgp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fehbvm.com/Article/details/gegnasmud.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fehbvm.com/Article/details/gdjehlavp.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.zdbjq.cn/Article/details/gxihktygt.sHtML

[R34] 退出时清理
来源：http://mobile.zdbjq.cn/Article/details/gijbiooyh.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gpgvwqxun.sHtML

[R35] 后台执行并等待
来源：http://baike.hesvh.cn/Article/details/ggkvxwvnq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fehbvm.com/Article/details/gkazdrmuc.sHtML

[R36] 并发执行多个任务
来源：http://m.share.hesvh.cn/Article/details/greecwfmn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.zdbjq.cn/Article/details/grkidxfpg.sHtML

[R37] 把输出赋给变量
来源：http://www.share.hesvh.cn/Article/details/gtfjjsnyt.sHtML

files=$(ls -1)
来源：http://wap.hesvh.cn/Article/details/gxljtxagv.sHtML

[R38] 管道串联
来源：http://baike.hesvh.cn/Article/details/ghsjzqsgt.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.zdbjq.cn/Article/details/gixcjusen.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.zdbjq.cn/Article/details/gsvlmiayo.sHtML

cmd > out.log 2>&1
来源：http://3g.zdbjq.cn/Article/details/gamttjmyw.sHtML

[R40] 追加写日志
来源：http://www.m.share.zdbjq.cn/Article/details/gytwqowba.sHtML

echo "log" >> out.log
来源：http://read.share.hesvh.cn/Article/details/gjituzpja.sHtML

[R41] 丢弃输出
来源：http://www.blog.zdbjq.cn/Article/details/ghcxiwdme.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/gigcdjnlb.sHtML

[R42] 输入重定向
来源：http://www.blog.zdbjq.cn/Article/details/grivpkjxn.sHtML

wc -l < a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gshjknsed.sHtML

[R43] 按名字查找文件
来源：http://www.share.zdbjq.cn/Article/details/gavetrnsa.sHtML

find . -name "*.log" -type f
来源：http://m.share.zdbjq.cn/Article/details/gwcsvawgn.sHtML

[R44] 按修改时间查找
来源：http://wap.hesvh.cn/Article/details/glhbcuhpm.sHtML

find . -mtime -7 -type f
来源：http://3g.zdbjq.cn/Article/details/guimwvbpj.sHtML

[R45] 批量删除
来源：http://blog.zdbjq.cn/Article/details/gcfmpnxaf.sHtML

find . -name "*.tmp" -delete
来源：http://blog.hesvh.cn/Article/details/gzzaikrdb.sHtML

[R46] 递归替换文件内容
来源：http://3g.fehbvm.com/Article/details/gaajfavph.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fehbvm.com/Article/details/gjqtnzxqo.sHtML

[R47] sed 单行替换
来源：http://baike.hesvh.cn/Article/details/grhhqdyvt.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.hesvh.cn/Article/details/gjvlndpjq.sHtML

[R48] awk 取指定列
来源：http://www.m.share.hesvh.cn/Article/details/gaqxvcvfj.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.zdbjq.cn/Article/details/gazloqake.sHtML

[R49] awk 带条件
来源：http://www.m.share.hesvh.cn/Article/details/gkhnqpmpr.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.hesvh.cn/Article/details/ghdhzuhsu.sHtML

[R50] awk 求和
来源：http://3g.fehbvm.com/Article/details/gtkhnbwdf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gxfnhzhwk.sHtML

[R51] 排序去重取前几
来源：http://blog.fehbvm.com/Article/details/gsmsqxstt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.zdbjq.cn/Article/details/gjluoyuue.sHtML

[R52] 统计行数
来源：http://3g.zdbjq.cn/Article/details/gbleyssnm.sHtML

wc -l a.txt
来源：http://m.share.fehbvm.com/Article/details/gkxdbiway.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.hesvh.cn/Article/details/gmdtykque.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fehbvm.com/Article/details/gwhaowwmf.sHtML

[R54] 比较两个文件
来源：http://www.blog.hesvh.cn/Article/details/gazhxkafx.sHtML

diff a.txt b.txt
来源：http://www.share.fehbvm.com/Article/details/gfibptlff.sHtML

[R55] 压缩与解压
来源：http://wap.hesvh.cn/Article/details/grxvihenx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.hesvh.cn/Article/details/guqtqmont.sHtML

[R56] 远程拷贝
来源：http://wap.hesvh.cn/Article/details/goemlptdg.sHtML

scp file user@host:/path/
来源：http://baike.hesvh.cn/Article/details/gaaexfxbt.sHtML

[R57] 远程执行命令
来源：http://www.m.share.hesvh.cn/Article/details/gecwtczvk.sHtML

ssh user@host 'uptime'
来源：http://3g.zdbjq.cn/Article/details/gdnlhsakc.sHtML

[R58] 下载文件
来源：http://www.m.share.zdbjq.cn/Article/details/gszjogqjn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fehbvm.com/Article/details/gvrszgasy.sHtML

[R59] 发 POST JSON
来源：http://blog.hesvh.cn/Article/details/gkddspwse.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.zdbjq.cn/Article/details/gazwqetlg.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/gyawzfxso.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fehbvm.com/Article/details/gucutxpan.sHtML

[R61] 磁盘占用
来源：http://read.share.hesvh.cn/Article/details/gyxqdfzym.sHtML

df -h;  du -sh *
来源：http://www.share.hesvh.cn/Article/details/gpzuyskyu.sHtML

[R62] 找最占空间的文件
来源：http://blog.hesvh.cn/Article/details/gfdcmdpam.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.zdbjq.cn/Article/details/ghrpiuiyw.sHtML

[R63] 内存与进程
来源：http://www.m.share.fehbvm.com/Article/details/girynagax.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.zdbjq.cn/Article/details/ghuvmlupa.sHtML

[R64] 结束进程
来源：http://m.share.fehbvm.com/Article/details/gxdslccaz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fehbvm.com/Article/details/gkkvbxexu.sHtML

[R65] 查看端口占用
来源：http://3g.zdbjq.cn/Article/details/gwbyfsqcq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fehbvm.com/Article/details/gqsudawqg.sHtML

[R66] 定时任务
来源：http://wap.zdbjq.cn/Article/details/gjevpvzig.sHtML

crontab -e;  crontab -l
来源：http://3g.zdbjq.cn/Article/details/gwxfqiyso.sHtML

[R67] 生成随机十六进制串
来源：http://3g.zdbjq.cn/Article/details/gmryipmgs.sHtML

openssl rand -hex 16
来源：http://3g.fehbvm.com/Article/details/gzvhaqqlu.sHtML

[R68] 计算文件校验值
来源：http://baike.zdbjq.cn/Article/details/gpvcalitm.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.hesvh.cn/Article/details/gwtrmumbm.sHtML

[R69] 生成随机密码
来源：http://baike.zdbjq.cn/Article/details/giwhzmfri.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.zdbjq.cn/Article/details/gajdcuqga.sHtML

[R70] 时间戳与互转
来源：http://m.share.hesvh.cn/Article/details/gjfkunudv.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fehbvm.com/Article/details/gkpczazwe.sHtML

[R71] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/gtkcjcuqm.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.zdbjq.cn/Article/details/gbhalbuim.sHtML

[R72] 等待端口就绪
来源：http://read.share.hesvh.cn/Article/details/gzokmzqpv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/gvzkdksim.sHtML

[R73] 分割大日志
来源：http://read.share.fehbvm.com/Article/details/gqhjnwwdo.sHtML

split -l 1000 big.log part_
来源：http://blog.zdbjq.cn/Article/details/gmbyfqisi.sHtML

[R74] 批量重命名
来源：http://baike.hesvh.cn/Article/details/goaxxuyiw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.zdbjq.cn/Article/details/gaptpkszs.sHtML

[R75] 导出环境变量
来源：http://www.share.zdbjq.cn/Article/details/gimakyjdq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.hesvh.cn/Article/details/gxgyhnwxe.sHtML

[R76] 使用临时文件
来源：http://baike.zdbjq.cn/Article/details/gcmsmppmu.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/gvpelkggo.sHtML

[R77] 读取用户输入
来源：http://wap.fehbvm.com/Article/details/gptiuzzxy.sHtML

read -rp "请输入: " ans
来源：http://3g.fehbvm.com/Article/details/grjbzayxl.sHtML

[R78] 交互式菜单
来源：http://read.share.zdbjq.cn/Article/details/gckeagxpj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.hesvh.cn/Article/details/gmblfrunz.sHtML

[R79] 解析命令行选项
来源：http://www.blog.zdbjq.cn/Article/details/gaqdyubwu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.hesvh.cn/Article/details/gyqutlett.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.zdbjq.cn/Article/details/gorabmsch.sHtML

time ./run.sh
来源：http://www.m.share.zdbjq.cn/Article/details/gclpdbqjl.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gvoqyhydn.sHtML

S. C / C++ 专题
来源：http://www.m.share.zdbjq.cn/Article/details/gkkpwmbnv.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gxodxkamd.sHtML

[S01] C：Hello World
来源：http://m.share.fehbvm.com/Article/details/genjcbuhj.sHtML

#include <stdio.h>
来源：http://wap.zdbjq.cn/Article/details/gnbkbcews.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fehbvm.com/Article/details/gyhwtqsjt.sHtML

[S02] C：变量与格式化输出
来源：http://blog.zdbjq.cn/Article/details/gdmtbejyx.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.hesvh.cn/Article/details/gmnnhlobd.sHtML

[S03] C：读入整数
来源：http://www.m.share.zdbjq.cn/Article/details/glgjxxbih.sHtML

int x; scanf("%d", &x);
来源：http://m.share.hesvh.cn/Article/details/gxnuyeeyy.sHtML

[S04] C：字符串复制
来源：http://www.m.share.hesvh.cn/Article/details/ginqyphba.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.hesvh.cn/Article/details/gliduyjab.sHtML

[S05] C：字符串长度
来源：http://3g.zdbjq.cn/Article/details/grzueizqw.sHtML

strlen(s)
来源：http://www.share.fehbvm.com/Article/details/gktwwckmw.sHtML

[S06] C：字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/glzpfsxim.sHtML

strcmp(a, b) == 0
来源：http://3g.zdbjq.cn/Article/details/gvebnmept.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fehbvm.com/Article/details/gmivvzewt.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.zdbjq.cn/Article/details/grxyqnzfh.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fehbvm.com/Article/details/gpoblxbdr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fehbvm.com/Article/details/gouhollkc.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.zdbjq.cn/Article/details/gxqcfrixb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fehbvm.com/Article/details/gwieehqbu.sHtML

[S10] C：指针与解引用
来源：http://baike.fehbvm.com/Article/details/gyzfbqkvx.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.zdbjq.cn/Article/details/gmwrwiqia.sHtML

[S11] C：逐行读文件
来源：http://blog.fehbvm.com/Article/details/grxmwepjp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.zdbjq.cn/Article/details/gmrzaagwo.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fehbvm.com/Article/details/gwfebntmi.sHtML

fclose(f);
来源：http://wap.hesvh.cn/Article/details/gdyilapgt.sHtML

[S12] C：写文件
来源：http://www.share.fehbvm.com/Article/details/gndvxmcte.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fehbvm.com/Article/details/gfqfwsmep.sHtML

[S13] C：宏定义
来源：http://mobile.hesvh.cn/Article/details/gqoroymxv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fehbvm.com/Article/details/gjyhjvptx.sHtML

[S14] C：枚举
来源：http://m.share.hesvh.cn/Article/details/gktscahuu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.hesvh.cn/Article/details/gqzilczto.sHtML

[S15] C：类型转换
来源：http://read.share.zdbjq.cn/Article/details/gvdtcduda.sHtML

(double) a / b
来源：http://m.share.zdbjq.cn/Article/details/gzbiasudi.sHtML

[S16] C：位操作置位
来源：http://wap.zdbjq.cn/Article/details/geeilcbur.sHtML

x |= (1 << 3);
来源：http://wap.hesvh.cn/Article/details/gtizapiqc.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gnsyhnnjh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.hesvh.cn/Article/details/gjgjajmgt.sHtML

[S18] C：命令行参数
来源：http://baike.hesvh.cn/Article/details/gqvxsjqzx.sHtML

int main(int argc, char **argv)
来源：http://wap.fehbvm.com/Article/details/gtglpefyr.sHtML

[S19] C：快速排序
来源：http://www.blog.hesvh.cn/Article/details/gkvfxdsrc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gjhadsgsp.sHtML

[S20] C：二分查找
来源：http://wap.fehbvm.com/Article/details/gfcwhixdc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gkqfztppy.sHtML

[S21] C：字符类别判断
来源：http://3g.fehbvm.com/Article/details/gnfivgqpq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.zdbjq.cn/Article/details/gzvhchwuo.sHtML

[S22] C：字符串转数字
来源：http://3g.zdbjq.cn/Article/details/giqasdjxk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.hesvh.cn/Article/details/goycrrsqy.sHtML

[S23] C：随机数
来源：http://3g.fehbvm.com/Article/details/gieacqhvl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fehbvm.com/Article/details/gxjmbxied.sHtML

[S24] C：获取本地时间
来源：http://www.blog.hesvh.cn/Article/details/guortwkel.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.hesvh.cn/Article/details/gszbihxab.sHtML

[S25] C：内存拷贝
来源：http://read.share.zdbjq.cn/Article/details/gqdwrrphv.sHtML

memcpy(dst, src, n);
来源：http://read.share.fehbvm.com/Article/details/gkbeqtkzp.sHtML

[S26] C：内存清零
来源：http://3g.hesvh.cn/Article/details/ggcddscsq.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.hesvh.cn/Article/details/gclxnkglq.sHtML

[S27] C：定义常量
来源：http://www.m.share.hesvh.cn/Article/details/gcuyvnniw.sHtML

const double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gjkodutur.sHtML

[S28] C：静态变量
来源：http://www.blog.fehbvm.com/Article/details/ghthrbedh.sHtML

static int counter = 0;
来源：http://www.blog.hesvh.cn/Article/details/gltidffrk.sHtML

[S29] C：变参函数
来源：http://mobile.zdbjq.cn/Article/details/gqnxbodvk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.zdbjq.cn/Article/details/gqszhdqnp.sHtML

[S30] C：头文件保护
来源：http://blog.fehbvm.com/Article/details/gpwlfduya.sHtML

#ifndef X_H
来源：http://m.share.hesvh.cn/Article/details/gnviixmnv.sHtML

#define X_H
来源：http://read.share.fehbvm.com/Article/details/gniyvesil.sHtML

#endif
来源：http://m.share.fehbvm.com/Article/details/gcglxckrx.sHtML

[S31] C++：Hello World
来源：http://www.blog.fehbvm.com/Article/details/goexqvphg.sHtML

#include <iostream>
来源：http://read.share.hesvh.cn/Article/details/gihzdkrou.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.zdbjq.cn/Article/details/gjnvbjule.sHtML

[S32] C++：字符串
来源：http://www.share.zdbjq.cn/Article/details/gmpuuwdxj.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.zdbjq.cn/Article/details/gviodlalv.sHtML

[S33] C++：vector 增删
来源：http://baike.hesvh.cn/Article/details/gfdtqjpdg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.zdbjq.cn/Article/details/gawbhjxxr.sHtML

[S34] C++：遍历 vector
来源：http://m.share.hesvh.cn/Article/details/gmwisavvc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.hesvh.cn/Article/details/gwhjwfvnf.sHtML

[S35] C++：map
来源：http://mobile.fehbvm.com/Article/details/gnscoamsi.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/gmvicifgg.sHtML

[S36] C++：unordered_map
来源：http://mobile.fehbvm.com/Article/details/gfnohpyvq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gsgzojfzc.sHtML

[S37] C++：set
来源：http://mobile.zdbjq.cn/Article/details/gszrdkxzd.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.zdbjq.cn/Article/details/gknqycebn.sHtML

[S38] C++：排序
来源：http://3g.fehbvm.com/Article/details/gdzobobao.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fehbvm.com/Article/details/gbxpifyun.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fehbvm.com/Article/details/guqiwatid.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.hesvh.cn/Article/details/gemrarehq.sHtML

[S40] C++：查找元素
来源：http://www.m.share.zdbjq.cn/Article/details/glcehspyr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fehbvm.com/Article/details/gbsphmwdy.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fehbvm.com/Article/details/gqaolkrmx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.zdbjq.cn/Article/details/gjtwcknri.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fehbvm.com/Article/details/gbuipqhjv.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.hesvh.cn/Article/details/gckyslnfy.sHtML

[S43] C++：智能指针
来源：http://read.share.fehbvm.com/Article/details/gyzrekebk.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fehbvm.com/Article/details/gczsgzrhe.sHtML

[S44] C++：引用传参
来源：http://www.share.hesvh.cn/Article/details/gmxhksukx.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fehbvm.com/Article/details/gediqkyne.sHtML

[S45] C++：lambda
来源：http://blog.zdbjq.cn/Article/details/gdvdecccs.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fehbvm.com/Article/details/gqwqwharr.sHtML

[S46] C++：函数模板
来源：http://www.blog.zdbjq.cn/Article/details/gixkizyfg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fehbvm.com/Article/details/gyyzpkwxz.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.zdbjq.cn/Article/details/gxxmtnkka.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.hesvh.cn/Article/details/ggsouocvf.sHtML

[S48] C++：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gqusksjxp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.zdbjq.cn/Article/details/gfcmlvvfd.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fehbvm.com/Article/details/gsdxhypvb.sHtML

[S49] C++：写文件
来源：http://m.share.zdbjq.cn/Article/details/gupefeias.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fehbvm.com/Article/details/gehziesye.sHtML

[S50] C++：格式化数字
来源：http://3g.fehbvm.com/Article/details/gczuspyni.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gdungmnyl.sHtML

[S51] C++：显式类型转换
来源：http://mobile.hesvh.cn/Article/details/gyxodusbk.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.zdbjq.cn/Article/details/genolitdw.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.zdbjq.cn/Article/details/gwxzojjes.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fehbvm.com/Article/details/gyrhnetnu.sHtML

[S53] C++：移动语义
来源：http://read.share.fehbvm.com/Article/details/gsvjxvnfk.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fehbvm.com/Article/details/gydgxlxvh.sHtML

[S54] C++：异常处理
来源：http://m.share.hesvh.cn/Article/details/goxnofafx.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.hesvh.cn/Article/details/gklcpewaq.sHtML

[S55] C++：结构化绑定
来源：http://wap.hesvh.cn/Article/details/gnmoqfjfj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.zdbjq.cn/Article/details/gwmcepueu.sHtML

[S56] C++：optional
来源：http://read.share.fehbvm.com/Article/details/gkufikwzv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.hesvh.cn/Article/details/gjacwrrtd.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.zdbjq.cn/Article/details/gnmoqdtvv.sHtML

constexpr int N = 10;
来源：http://mobile.zdbjq.cn/Article/details/ggzvymjcr.sHtML

[S58] C++：命名空间
来源：http://baike.hesvh.cn/Article/details/gcbmnuvlp.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.hesvh.cn/Article/details/gqlwkglzp.sHtML

[S59] C++：静态断言
来源：http://baike.fehbvm.com/Article/details/gforsbljb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.hesvh.cn/Article/details/ghujilsks.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.zdbjq.cn/Article/details/gpzsksupc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.zdbjq.cn/Article/details/gkvwcgwjg.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gcvxilegz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.hesvh.cn/Article/details/gypxgjgkv.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gxjeozvcj.sHtML

[T01] Kotlin：Hello World
来源：http://3g.hesvh.cn/Article/details/gmwzslelh.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/gsulkwdlq.sHtML

[T02] Kotlin：变量
来源：http://www.share.hesvh.cn/Article/details/gpmykpzlm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fehbvm.com/Article/details/gkrtawesw.sHtML


<!-- 参考信息 -->