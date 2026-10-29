代发 wailian999

esac
来源：http://read.share.zdbjq.cn/Article/details/gfjqxszdz.sHtML

[R12] for 遍历文件
来源：http://m.share.fehbvm.com/Article/details/gjwzvlsfk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fehbvm.com/Article/details/gmskmsvjb.sHtML

[R13] for 计数循环
来源：http://3g.zdbjq.cn/Article/details/gqfuerddz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/gbsqmcdeu.sHtML

[R14] C 风格 for
来源：http://3g.fehbvm.com/Article/details/gqpqepfhk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/ghuferlgm.sHtML

[R15] while 逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gidjpcirc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.hesvh.cn/Article/details/gawnxihqg.sHtML

[R16] until 等待条件
来源：http://www.blog.hesvh.cn/Article/details/gaxxvlene.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/glijjmaxc.sHtML

[R17] 数组定义与取值
来源：http://mobile.zdbjq.cn/Article/details/gpxrrqses.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.zdbjq.cn/Article/details/gngrhjzpf.sHtML

[R18] 遍历数组
来源：http://read.share.zdbjq.cn/Article/details/gpnyyuege.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fehbvm.com/Article/details/ggwwvafst.sHtML

[R19] 数组长度
来源：http://www.share.fehbvm.com/Article/details/gputbyjsb.sHtML

echo "${#arr[@]}"
来源：http://mobile.fehbvm.com/Article/details/gocakmfix.sHtML

[R20] 关联数组（字典）
来源：http://m.share.hesvh.cn/Article/details/gtjgoticr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.zdbjq.cn/Article/details/gbadplvjw.sHtML

[R21] 字符串长度
来源：http://read.share.fehbvm.com/Article/details/gaxnzzdtb.sHtML

echo "${#s}"
来源：http://www.m.share.fehbvm.com/Article/details/gkasueqoz.sHtML

[R22] 截取子串
来源：http://blog.hesvh.cn/Article/details/gkqijhqsh.sHtML

echo "${s:0:5}"
来源：http://blog.hesvh.cn/Article/details/ggoieaodm.sHtML

[R23] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/ggivevtbo.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fehbvm.com/Article/details/gpmsrrtns.sHtML

[R24] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gxiozljxv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fehbvm.com/Article/details/gwddtpbbq.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.hesvh.cn/Article/details/ggbdfrhmc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.zdbjq.cn/Article/details/gwwaqirwh.sHtML

[R26] 命令替换
来源：http://3g.fehbvm.com/Article/details/goomdeqau.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.zdbjq.cn/Article/details/gmrhyvucr.sHtML

[R27] 算术展开
来源：http://baike.zdbjq.cn/Article/details/gxmpozqei.sHtML

echo $((1 + 2 * 3))
来源：http://wap.zdbjq.cn/Article/details/gldvywfno.sHtML

[R28] 浮点运算
来源：http://blog.hesvh.cn/Article/details/gsluogztp.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.hesvh.cn/Article/details/gbwdlixep.sHtML

[R29] 定义函数
来源：http://www.share.fehbvm.com/Article/details/geshombbk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.zdbjq.cn/Article/details/gkiiqlaxk.sHtML

[R30] 函数返回状态码
来源：http://read.share.hesvh.cn/Article/details/gtqrhdsea.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.zdbjq.cn/Article/details/grjvdrlcv.sHtML

[R31] 局部变量
来源：http://read.share.hesvh.cn/Article/details/gkumjnhva.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.hesvh.cn/Article/details/gqyyotfhk.sHtML

[R32] 参数个数校验
来源：http://mobile.hesvh.cn/Article/details/gszftgibg.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gbahorzua.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.zdbjq.cn/Article/details/gcmppssmv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.zdbjq.cn/Article/details/gdzjaiqvs.sHtML

[R34] 退出时清理
来源：http://blog.hesvh.cn/Article/details/gdyyoyzkz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/glgnlkjft.sHtML

[R35] 后台执行并等待
来源：http://read.share.zdbjq.cn/Article/details/gccskptsq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.zdbjq.cn/Article/details/gxyvwtyxc.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.zdbjq.cn/Article/details/gdrtvvjqa.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.zdbjq.cn/Article/details/gqcuszyeb.sHtML

[R37] 把输出赋给变量
来源：http://m.share.zdbjq.cn/Article/details/gaoycgkia.sHtML

files=$(ls -1)
来源：http://mobile.fehbvm.com/Article/details/gmglwoswx.sHtML

[R38] 管道串联
来源：http://blog.fehbvm.com/Article/details/glfbifhln.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.zdbjq.cn/Article/details/gxvqvgayr.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fehbvm.com/Article/details/gyapmhdbg.sHtML

cmd > out.log 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/gnwevxytf.sHtML

[R40] 追加写日志
来源：http://m.share.hesvh.cn/Article/details/gxyzsjoen.sHtML

echo "log" >> out.log
来源：http://m.share.hesvh.cn/Article/details/gdlbmggaz.sHtML

[R41] 丢弃输出
来源：http://www.blog.zdbjq.cn/Article/details/gwgnaqsqj.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fehbvm.com/Article/details/ghextoskv.sHtML

[R42] 输入重定向
来源：http://3g.fehbvm.com/Article/details/ggpbzzprx.sHtML

wc -l < a.txt
来源：http://mobile.zdbjq.cn/Article/details/gvorkzcxt.sHtML

[R43] 按名字查找文件
来源：http://mobile.hesvh.cn/Article/details/goyaojyhb.sHtML

find . -name "*.log" -type f
来源：http://3g.fehbvm.com/Article/details/grvchixqo.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.hesvh.cn/Article/details/grggqlzzs.sHtML

find . -mtime -7 -type f
来源：http://mobile.zdbjq.cn/Article/details/gtwcwuyrm.sHtML

[R45] 批量删除
来源：http://m.share.hesvh.cn/Article/details/gbjhzulto.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fehbvm.com/Article/details/gxoxfewpg.sHtML

[R46] 递归替换文件内容
来源：http://blog.zdbjq.cn/Article/details/gzkajxzch.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.zdbjq.cn/Article/details/gltpxtkng.sHtML

[R47] sed 单行替换
来源：http://read.share.fehbvm.com/Article/details/gzvekpjat.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.hesvh.cn/Article/details/gvhfanfci.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fehbvm.com/Article/details/gbpjjgyaj.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gttbghzpg.sHtML

[R49] awk 带条件
来源：http://mobile.fehbvm.com/Article/details/gsvnqztko.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fehbvm.com/Article/details/ghkvwsowg.sHtML

[R50] awk 求和
来源：http://m.share.zdbjq.cn/Article/details/gnukcbjsd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fehbvm.com/Article/details/gbehkntew.sHtML

[R51] 排序去重取前几
来源：http://mobile.fehbvm.com/Article/details/gmmooufub.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.zdbjq.cn/Article/details/gkkewttvv.sHtML

[R52] 统计行数
来源：http://m.share.zdbjq.cn/Article/details/gjehowaau.sHtML

wc -l a.txt
来源：http://wap.hesvh.cn/Article/details/grolvrzli.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.hesvh.cn/Article/details/gnesnagex.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.hesvh.cn/Article/details/gendtofct.sHtML

[R54] 比较两个文件
来源：http://m.share.hesvh.cn/Article/details/gmqsvtnbl.sHtML

diff a.txt b.txt
来源：http://blog.zdbjq.cn/Article/details/gslbumfwy.sHtML

[R55] 压缩与解压
来源：http://3g.hesvh.cn/Article/details/gnelmyvtg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fehbvm.com/Article/details/grxbmjavx.sHtML

[R56] 远程拷贝
来源：http://www.share.hesvh.cn/Article/details/grxrnzsbr.sHtML

scp file user@host:/path/
来源：http://blog.hesvh.cn/Article/details/ggrfewrfn.sHtML

[R57] 远程执行命令
来源：http://baike.fehbvm.com/Article/details/gdawbqhup.sHtML

ssh user@host 'uptime'
来源：http://blog.zdbjq.cn/Article/details/grfdpfouo.sHtML

[R58] 下载文件
来源：http://blog.hesvh.cn/Article/details/gjvmdviyh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.zdbjq.cn/Article/details/gwakcqmvd.sHtML

[R59] 发 POST JSON
来源：http://www.share.zdbjq.cn/Article/details/gsjuttzjt.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.zdbjq.cn/Article/details/gbhgurnxi.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/gqerheirx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fehbvm.com/Article/details/gmiuqerms.sHtML

[R61] 磁盘占用
来源：http://m.share.hesvh.cn/Article/details/gjaidzwkg.sHtML

df -h;  du -sh *
来源：http://m.share.hesvh.cn/Article/details/gtsiohpch.sHtML

[R62] 找最占空间的文件
来源：http://blog.zdbjq.cn/Article/details/gxbeqnwup.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.hesvh.cn/Article/details/gwhqafslq.sHtML

[R63] 内存与进程
来源：http://3g.zdbjq.cn/Article/details/galtuvbqt.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.hesvh.cn/Article/details/gpqwqcavj.sHtML

[R64] 结束进程
来源：http://www.share.fehbvm.com/Article/details/gtwgmolfv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.zdbjq.cn/Article/details/gpoiskgic.sHtML

[R65] 查看端口占用
来源：http://read.share.hesvh.cn/Article/details/gsxyegapt.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.zdbjq.cn/Article/details/gfbhcacet.sHtML

[R66] 定时任务
来源：http://www.blog.zdbjq.cn/Article/details/gcytmgurn.sHtML

crontab -e;  crontab -l
来源：http://m.share.fehbvm.com/Article/details/gplecqjmw.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fehbvm.com/Article/details/gwlirlhsr.sHtML

openssl rand -hex 16
来源：http://wap.hesvh.cn/Article/details/gsevrbijc.sHtML

[R68] 计算文件校验值
来源：http://m.share.zdbjq.cn/Article/details/gadtxzylg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.hesvh.cn/Article/details/gfvaszyrf.sHtML

[R69] 生成随机密码
来源：http://m.share.fehbvm.com/Article/details/ghopnkudn.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fehbvm.com/Article/details/gazpjiypy.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.zdbjq.cn/Article/details/gzckmcvzc.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fehbvm.com/Article/details/gkzpggxxc.sHtML

[R71] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gkfsriytk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.zdbjq.cn/Article/details/gcdhehpvp.sHtML

[R72] 等待端口就绪
来源：http://baike.fehbvm.com/Article/details/glyhwtzgc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/gcfczpenr.sHtML

[R73] 分割大日志
来源：http://www.blog.fehbvm.com/Article/details/gnfbgjkls.sHtML

split -l 1000 big.log part_
来源：http://mobile.hesvh.cn/Article/details/gfbweuvet.sHtML

[R74] 批量重命名
来源：http://baike.zdbjq.cn/Article/details/gexstqhpx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.zdbjq.cn/Article/details/ggqygqgpp.sHtML

[R75] 导出环境变量
来源：http://m.share.zdbjq.cn/Article/details/gtmfudyqd.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fehbvm.com/Article/details/gfiixeanh.sHtML

[R76] 使用临时文件
来源：http://www.share.hesvh.cn/Article/details/gncbjnpip.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/ghigmplni.sHtML

[R77] 读取用户输入
来源：http://3g.hesvh.cn/Article/details/gzsqdoiqm.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.zdbjq.cn/Article/details/gxxsmzbdx.sHtML

[R78] 交互式菜单
来源：http://m.share.fehbvm.com/Article/details/glimutwyc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.hesvh.cn/Article/details/glqmyhyju.sHtML

[R79] 解析命令行选项
来源：http://m.share.zdbjq.cn/Article/details/gnhrnzvfj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.hesvh.cn/Article/details/gnpovpyni.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fehbvm.com/Article/details/gyzjphiqj.sHtML

time ./run.sh
来源：http://www.share.fehbvm.com/Article/details/gaqtpdrbp.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gwsjsguwx.sHtML

S. C / C++ 专题
来源：http://baike.zdbjq.cn/Article/details/gjcslkelw.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gdjyurytb.sHtML

[S01] C：Hello World
来源：http://m.share.hesvh.cn/Article/details/goxhnmyse.sHtML

#include <stdio.h>
来源：http://wap.hesvh.cn/Article/details/gyujornss.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.zdbjq.cn/Article/details/gzhnhxtza.sHtML

[S02] C：变量与格式化输出
来源：http://baike.zdbjq.cn/Article/details/ghcikbafp.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.zdbjq.cn/Article/details/gjnvyikyi.sHtML

[S03] C：读入整数
来源：http://mobile.fehbvm.com/Article/details/gungqqzyz.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.hesvh.cn/Article/details/ggfiufmmw.sHtML

[S04] C：字符串复制
来源：http://www.share.fehbvm.com/Article/details/gfozeuzng.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.hesvh.cn/Article/details/gncqapasn.sHtML

[S05] C：字符串长度
来源：http://3g.zdbjq.cn/Article/details/gnphqakaq.sHtML

strlen(s)
来源：http://wap.zdbjq.cn/Article/details/geiegcypl.sHtML

[S06] C：字符串比较
来源：http://read.share.zdbjq.cn/Article/details/glcpdodkt.sHtML

strcmp(a, b) == 0
来源：http://m.share.hesvh.cn/Article/details/gwlgehriy.sHtML

[S07] C：数组遍历求和
来源：http://read.share.zdbjq.cn/Article/details/gfkeygjyo.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fehbvm.com/Article/details/gyddfkoic.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.zdbjq.cn/Article/details/geyejqpzo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.zdbjq.cn/Article/details/gqekynozv.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fehbvm.com/Article/details/gdvttpdmn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.zdbjq.cn/Article/details/gfrhbzrms.sHtML

[S10] C：指针与解引用
来源：http://m.share.zdbjq.cn/Article/details/ggdpposqe.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.hesvh.cn/Article/details/gppikjwzc.sHtML

[S11] C：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gakknrzak.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.hesvh.cn/Article/details/gggkirbwu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fehbvm.com/Article/details/gjrsexalo.sHtML

fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gnoxtbyju.sHtML

[S12] C：写文件
来源：http://read.share.zdbjq.cn/Article/details/gjvksznwa.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gtysppyva.sHtML

[S13] C：宏定义
来源：http://baike.hesvh.cn/Article/details/gullwkxpx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.zdbjq.cn/Article/details/giwskjclq.sHtML

[S14] C：枚举
来源：http://blog.hesvh.cn/Article/details/gthejvtln.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.zdbjq.cn/Article/details/gygguqkod.sHtML

[S15] C：类型转换
来源：http://www.share.zdbjq.cn/Article/details/gylfcnsaz.sHtML

(double) a / b
来源：http://mobile.hesvh.cn/Article/details/glqlxehdb.sHtML

[S16] C：位操作置位
来源：http://www.share.zdbjq.cn/Article/details/gvsdrfblo.sHtML

x |= (1 << 3);
来源：http://read.share.fehbvm.com/Article/details/gvkgthgbh.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/garxamhzs.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.zdbjq.cn/Article/details/gmusjzequ.sHtML

[S18] C：命令行参数
来源：http://www.share.zdbjq.cn/Article/details/ghkyxwnvv.sHtML

int main(int argc, char **argv)
来源：http://mobile.hesvh.cn/Article/details/gpoykkzft.sHtML

[S19] C：快速排序
来源：http://wap.fehbvm.com/Article/details/gyjnjdggb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/gdbpvguuj.sHtML

[S20] C：二分查找
来源：http://www.share.zdbjq.cn/Article/details/gjuyasbfn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/gcuklbsde.sHtML

[S21] C：字符类别判断
来源：http://mobile.zdbjq.cn/Article/details/gzfrdmfce.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.zdbjq.cn/Article/details/gxpzjlaco.sHtML

[S22] C：字符串转数字
来源：http://www.share.hesvh.cn/Article/details/gcwisvore.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.zdbjq.cn/Article/details/gdrwbnuni.sHtML

[S23] C：随机数
来源：http://wap.zdbjq.cn/Article/details/gdpsqilgo.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.hesvh.cn/Article/details/gseynkagf.sHtML

[S24] C：获取本地时间
来源：http://m.share.fehbvm.com/Article/details/gfgjbyvat.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.zdbjq.cn/Article/details/ggrwrykpo.sHtML

[S25] C：内存拷贝
来源：http://www.share.fehbvm.com/Article/details/gqsamqofj.sHtML

memcpy(dst, src, n);
来源：http://wap.hesvh.cn/Article/details/gubawtqlo.sHtML

[S26] C：内存清零
来源：http://3g.fehbvm.com/Article/details/gyjivlqiu.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fehbvm.com/Article/details/gmwtxqsjh.sHtML

[S27] C：定义常量
来源：http://www.share.zdbjq.cn/Article/details/gtmhnfrmp.sHtML

const double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/glahjwvnu.sHtML

[S28] C：静态变量
来源：http://baike.zdbjq.cn/Article/details/galooouwm.sHtML

static int counter = 0;
来源：http://m.share.fehbvm.com/Article/details/gfhibxyhp.sHtML

[S29] C：变参函数
来源：http://blog.fehbvm.com/Article/details/gpsfbgmxb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.zdbjq.cn/Article/details/gqutbdvan.sHtML

[S30] C：头文件保护
来源：http://www.share.hesvh.cn/Article/details/gohenyluv.sHtML

#ifndef X_H
来源：http://www.blog.hesvh.cn/Article/details/gmqglwzor.sHtML

#define X_H
来源：http://blog.zdbjq.cn/Article/details/gfchqgxly.sHtML

#endif
来源：http://m.share.zdbjq.cn/Article/details/gyiizxkeg.sHtML

[S31] C++：Hello World
来源：http://www.share.zdbjq.cn/Article/details/goagsirqh.sHtML

#include <iostream>
来源：http://wap.hesvh.cn/Article/details/gocbbhbwk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.hesvh.cn/Article/details/gdcjrhkcf.sHtML

[S32] C++：字符串
来源：http://www.m.share.fehbvm.com/Article/details/gmnxgccvp.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.hesvh.cn/Article/details/gdbckhxqz.sHtML

[S33] C++：vector 增删
来源：http://m.share.hesvh.cn/Article/details/gsfcomlee.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.zdbjq.cn/Article/details/gvauxixti.sHtML

[S34] C++：遍历 vector
来源：http://wap.zdbjq.cn/Article/details/gyydelpir.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fehbvm.com/Article/details/gtmggpohd.sHtML

[S35] C++：map
来源：http://m.share.hesvh.cn/Article/details/gqlogsksx.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gexsxapnm.sHtML

[S36] C++：unordered_map
来源：http://3g.zdbjq.cn/Article/details/ghkfmqrlp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/goosdzfpg.sHtML

[S37] C++：set
来源：http://mobile.hesvh.cn/Article/details/gmeqhjsia.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.hesvh.cn/Article/details/gczvboyyz.sHtML

[S38] C++：排序
来源：http://www.share.hesvh.cn/Article/details/gibvgjztn.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/gpplfuprm.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fehbvm.com/Article/details/ggxtoqamy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.hesvh.cn/Article/details/ghucyhnxs.sHtML

[S40] C++：查找元素
来源：http://3g.zdbjq.cn/Article/details/gnghkaucl.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fehbvm.com/Article/details/gvolcdlcf.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fehbvm.com/Article/details/gwlurslii.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.hesvh.cn/Article/details/gmupagccg.sHtML

[S42] C++：继承与虚函数
来源：http://blog.zdbjq.cn/Article/details/gjmofbwoz.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.hesvh.cn/Article/details/gjccwvjwm.sHtML

[S43] C++：智能指针
来源：http://mobile.fehbvm.com/Article/details/gytpuchjc.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fehbvm.com/Article/details/goenvnrsm.sHtML

[S44] C++：引用传参
来源：http://mobile.fehbvm.com/Article/details/gxsmbyzhd.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.hesvh.cn/Article/details/gpzcroeag.sHtML

[S45] C++：lambda
来源：http://read.share.zdbjq.cn/Article/details/giieqdjzg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.hesvh.cn/Article/details/gashehwgw.sHtML

[S46] C++：函数模板
来源：http://wap.fehbvm.com/Article/details/gkhuzbytp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.zdbjq.cn/Article/details/gupvrlxyt.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gthileedg.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.zdbjq.cn/Article/details/gjaccmstb.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/ghwxoqpqt.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fehbvm.com/Article/details/gddtdewyq.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fehbvm.com/Article/details/ghfvebvyx.sHtML

[S49] C++：写文件
来源：http://blog.fehbvm.com/Article/details/gzxdpisyq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.hesvh.cn/Article/details/gkprfaabn.sHtML

[S50] C++：格式化数字
来源：http://www.blog.hesvh.cn/Article/details/gxqzzlhks.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gytthpcpp.sHtML

[S51] C++：显式类型转换
来源：http://m.share.hesvh.cn/Article/details/grnnatqoh.sHtML

static_cast<double>(a) / b
来源：http://www.share.fehbvm.com/Article/details/gpwygbmcw.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.zdbjq.cn/Article/details/gfodwesxh.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.hesvh.cn/Article/details/gecwznkpk.sHtML

[S53] C++：移动语义
来源：http://blog.zdbjq.cn/Article/details/gvziidwqk.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.hesvh.cn/Article/details/gjsjpohsq.sHtML

[S54] C++：异常处理
来源：http://wap.zdbjq.cn/Article/details/gtuckidkx.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.hesvh.cn/Article/details/ghytimqow.sHtML

[S55] C++：结构化绑定
来源：http://m.share.hesvh.cn/Article/details/glasinrmj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fehbvm.com/Article/details/gmkvavntw.sHtML

[S56] C++：optional
来源：http://mobile.zdbjq.cn/Article/details/ghqswwagu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.hesvh.cn/Article/details/gxeyzzksg.sHtML

[S57] C++：编译期常量
来源：http://baike.fehbvm.com/Article/details/guchtsnxh.sHtML

constexpr int N = 10;
来源：http://blog.fehbvm.com/Article/details/gmrrnihha.sHtML

[S58] C++：命名空间
来源：http://blog.zdbjq.cn/Article/details/gnfoftyjb.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.hesvh.cn/Article/details/gkfqmxfxb.sHtML

[S59] C++：静态断言
来源：http://3g.hesvh.cn/Article/details/gmpverpxm.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fehbvm.com/Article/details/gemezgpzd.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.hesvh.cn/Article/details/gmnqqnpjv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.hesvh.cn/Article/details/gczmugdac.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gqvlotwst.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.zdbjq.cn/Article/details/gjacwkzjt.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gkwvoffph.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gbwbqhucv.sHtML

println("Hello")
来源：http://read.share.hesvh.cn/Article/details/ghckrshvl.sHtML

[T02] Kotlin：变量
来源：http://blog.hesvh.cn/Article/details/gkepfhphr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.hesvh.cn/Article/details/gvctahilv.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.zdbjq.cn/Article/details/gyqknjklb.sHtML

"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/gwuttaxqa.sHtML

[T04] Kotlin：空安全
来源：http://wap.hesvh.cn/Article/details/gzgjctlyu.sHtML

val n: String? = null;  n?.length
来源：http://mobile.hesvh.cn/Article/details/glbtksfvj.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.hesvh.cn/Article/details/glycivggl.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fehbvm.com/Article/details/gqcycwtil.sHtML

[T06] Kotlin：集合映射
来源：http://wap.zdbjq.cn/Article/details/gnhzsqynb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.zdbjq.cn/Article/details/gfhhqxqhi.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/gxzgfyyck.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fehbvm.com/Article/details/ginsqnnug.sHtML

[T08] Kotlin：数据类
来源：http://mobile.hesvh.cn/Article/details/gxomllbfe.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.hesvh.cn/Article/details/gdqiyrujc.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fehbvm.com/Article/details/ghxnyuqto.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.hesvh.cn/Article/details/gvenjeuef.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.zdbjq.cn/Article/details/gaxiiqtis.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.zdbjq.cn/Article/details/gewcxxgse.sHtML

[T11] Kotlin：协程
来源：http://baike.hesvh.cn/Article/details/gwfbibsax.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fehbvm.com/Article/details/gyczgrnvr.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fehbvm.com/Article/details/guwffwfdt.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gbuytcfru.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.zdbjq.cn/Article/details/ggopfeini.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.hesvh.cn/Article/details/gjxuikjsh.sHtML

[T14] Kotlin：循环
来源：http://blog.fehbvm.com/Article/details/ghyaxmoyv.sHtML

for (i in 1..10) println(i)
来源：http://wap.hesvh.cn/Article/details/glbmaghkt.sHtML


<!-- 参考信息 -->