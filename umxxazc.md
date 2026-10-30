代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.zdbjq.cn/Article/details/gfdlqwvje.sHtML

[R18] 遍历数组
来源：http://wap.fehbvm.com/Article/details/gjxgzhinh.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fehbvm.com/Article/details/gwgqfbiwb.sHtML

[R19] 数组长度
来源：http://m.share.hesvh.cn/Article/details/gnynjfyjb.sHtML

echo "${#arr[@]}"
来源：http://mobile.hesvh.cn/Article/details/gzvfwfsfw.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.hesvh.cn/Article/details/gffqcmnkb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fehbvm.com/Article/details/gpzlppqep.sHtML

[R21] 字符串长度
来源：http://baike.hesvh.cn/Article/details/gohibdkoy.sHtML

echo "${#s}"
来源：http://wap.hesvh.cn/Article/details/gswxvaoyj.sHtML

[R22] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/gbmnvlwni.sHtML

echo "${s:0:5}"
来源：http://read.share.zdbjq.cn/Article/details/gajwddyds.sHtML

[R23] 字符串替换
来源：http://baike.hesvh.cn/Article/details/gibucwegy.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fehbvm.com/Article/details/gxumnxfon.sHtML

[R24] 大小写转换
来源：http://blog.hesvh.cn/Article/details/gxshoplln.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fehbvm.com/Article/details/gndrhhjbl.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.hesvh.cn/Article/details/gkargspzt.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.zdbjq.cn/Article/details/gwnvmhfst.sHtML

[R26] 命令替换
来源：http://mobile.hesvh.cn/Article/details/grqezmzwg.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.hesvh.cn/Article/details/gfefzzsoj.sHtML

[R27] 算术展开
来源：http://baike.hesvh.cn/Article/details/gwfbozkqi.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.zdbjq.cn/Article/details/gokyaprxw.sHtML

[R28] 浮点运算
来源：http://baike.hesvh.cn/Article/details/grgsxmvko.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.zdbjq.cn/Article/details/gysuvlqyv.sHtML

[R29] 定义函数
来源：http://3g.zdbjq.cn/Article/details/ghveloltz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fehbvm.com/Article/details/gxllfocfy.sHtML

[R30] 函数返回状态码
来源：http://read.share.fehbvm.com/Article/details/gknqksdbu.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.hesvh.cn/Article/details/ggxjxttlm.sHtML

[R31] 局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gcadnxpfo.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fehbvm.com/Article/details/gebapmmjr.sHtML

[R32] 参数个数校验
来源：http://mobile.zdbjq.cn/Article/details/gqohqqzwt.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/gvajwgzeu.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.hesvh.cn/Article/details/goabnwppu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.zdbjq.cn/Article/details/gbfzizvhp.sHtML

[R34] 退出时清理
来源：http://3g.fehbvm.com/Article/details/gcjdddvxa.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/ghklfihhd.sHtML

[R35] 后台执行并等待
来源：http://blog.hesvh.cn/Article/details/ggefvmcoi.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.hesvh.cn/Article/details/gpnrvppjg.sHtML

[R36] 并发执行多个任务
来源：http://wap.fehbvm.com/Article/details/gwmzzumqc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.hesvh.cn/Article/details/gqqjhcwdn.sHtML

[R37] 把输出赋给变量
来源：http://wap.zdbjq.cn/Article/details/gawonnbdf.sHtML

files=$(ls -1)
来源：http://www.share.hesvh.cn/Article/details/gtkygfioa.sHtML

[R38] 管道串联
来源：http://m.share.hesvh.cn/Article/details/gnnutzhal.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.hesvh.cn/Article/details/gclhsfuqk.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fehbvm.com/Article/details/gvijcebpx.sHtML

cmd > out.log 2>&1
来源：http://baike.fehbvm.com/Article/details/gnjuyjaam.sHtML

[R40] 追加写日志
来源：http://wap.fehbvm.com/Article/details/gzrwcpobv.sHtML

echo "log" >> out.log
来源：http://mobile.fehbvm.com/Article/details/gyuhnksjf.sHtML

[R41] 丢弃输出
来源：http://3g.fehbvm.com/Article/details/ganlehuip.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/gtebrnqen.sHtML

[R42] 输入重定向
来源：http://mobile.fehbvm.com/Article/details/gkmxohsdk.sHtML

wc -l < a.txt
来源：http://www.blog.zdbjq.cn/Article/details/glrjhcewg.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fehbvm.com/Article/details/gzmcywvla.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fehbvm.com/Article/details/gibifpghz.sHtML

[R44] 按修改时间查找
来源：http://www.share.fehbvm.com/Article/details/gvtbjtcve.sHtML

find . -mtime -7 -type f
来源：http://baike.hesvh.cn/Article/details/gooleaxad.sHtML

[R45] 批量删除
来源：http://3g.hesvh.cn/Article/details/gknylbwdu.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fehbvm.com/Article/details/gqpvxxjrz.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.hesvh.cn/Article/details/ghjdgsvud.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.hesvh.cn/Article/details/gyaywehri.sHtML

[R47] sed 单行替换
来源：http://blog.zdbjq.cn/Article/details/guwjvyklb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gpplagsnp.sHtML

[R48] awk 取指定列
来源：http://read.share.zdbjq.cn/Article/details/gxdlmansx.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gutimjjbu.sHtML

[R49] awk 带条件
来源：http://read.share.zdbjq.cn/Article/details/grzjgpnmf.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.zdbjq.cn/Article/details/gnnwfvpng.sHtML

[R50] awk 求和
来源：http://blog.hesvh.cn/Article/details/gnlihozuq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fehbvm.com/Article/details/gjheoiaoj.sHtML

[R51] 排序去重取前几
来源：http://blog.zdbjq.cn/Article/details/gxecbheam.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fehbvm.com/Article/details/gdtppnsiu.sHtML

[R52] 统计行数
来源：http://blog.zdbjq.cn/Article/details/gfbzjdpub.sHtML

wc -l a.txt
来源：http://read.share.hesvh.cn/Article/details/gpyldevds.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.zdbjq.cn/Article/details/gzexhrnrq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fehbvm.com/Article/details/gqsiztrzb.sHtML

[R54] 比较两个文件
来源：http://mobile.zdbjq.cn/Article/details/gszfymubp.sHtML

diff a.txt b.txt
来源：http://blog.fehbvm.com/Article/details/gnalxfzii.sHtML

[R55] 压缩与解压
来源：http://blog.zdbjq.cn/Article/details/gauwjflhi.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.hesvh.cn/Article/details/gqeqimxbu.sHtML

[R56] 远程拷贝
来源：http://www.share.fehbvm.com/Article/details/gqyqfpncg.sHtML

scp file user@host:/path/
来源：http://www.share.hesvh.cn/Article/details/gdxgppgev.sHtML

[R57] 远程执行命令
来源：http://m.share.zdbjq.cn/Article/details/gekkketrp.sHtML

ssh user@host 'uptime'
来源：http://read.share.hesvh.cn/Article/details/gvatlpqcj.sHtML

[R58] 下载文件
来源：http://www.blog.zdbjq.cn/Article/details/grxhhamut.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fehbvm.com/Article/details/gpztznqtp.sHtML

[R59] 发 POST JSON
来源：http://wap.fehbvm.com/Article/details/ghqaykppp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fehbvm.com/Article/details/gwdjfktgz.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/gcffcbdrm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.zdbjq.cn/Article/details/gcifnpmwm.sHtML

[R61] 磁盘占用
来源：http://3g.fehbvm.com/Article/details/gncaytnnf.sHtML

df -h;  du -sh *
来源：http://www.share.zdbjq.cn/Article/details/gbnkxdoyb.sHtML

[R62] 找最占空间的文件
来源：http://wap.fehbvm.com/Article/details/gobxotvhd.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.hesvh.cn/Article/details/ggjzyjfqq.sHtML

[R63] 内存与进程
来源：http://www.blog.fehbvm.com/Article/details/gmqrxayij.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.zdbjq.cn/Article/details/gkerbojja.sHtML

[R64] 结束进程
来源：http://mobile.fehbvm.com/Article/details/gbvaqkomu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.zdbjq.cn/Article/details/gvtghipjp.sHtML

[R65] 查看端口占用
来源：http://m.share.hesvh.cn/Article/details/giagvrmnm.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fehbvm.com/Article/details/gvgnlrbil.sHtML

[R66] 定时任务
来源：http://mobile.zdbjq.cn/Article/details/ghvzlsgrq.sHtML

crontab -e;  crontab -l
来源：http://www.share.hesvh.cn/Article/details/gexxmdgjb.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fehbvm.com/Article/details/gknjvovge.sHtML

openssl rand -hex 16
来源：http://mobile.zdbjq.cn/Article/details/gjqfjgvwe.sHtML

[R68] 计算文件校验值
来源：http://www.share.zdbjq.cn/Article/details/glzrqkcjg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/giiibfrey.sHtML

[R69] 生成随机密码
来源：http://baike.fehbvm.com/Article/details/gsqneriqe.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.hesvh.cn/Article/details/glsiqoexn.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.zdbjq.cn/Article/details/gowickpcl.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.hesvh.cn/Article/details/gxlgkppom.sHtML

[R71] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/giprivlpm.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.zdbjq.cn/Article/details/gpyuzfvun.sHtML

[R72] 等待端口就绪
来源：http://3g.hesvh.cn/Article/details/gaxhnobml.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/gwaxlvhvt.sHtML

[R73] 分割大日志
来源：http://baike.fehbvm.com/Article/details/gtuupnvxj.sHtML

split -l 1000 big.log part_
来源：http://www.blog.zdbjq.cn/Article/details/ghohiqtiu.sHtML

[R74] 批量重命名
来源：http://wap.zdbjq.cn/Article/details/gqgeniifb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.zdbjq.cn/Article/details/gdnclvldo.sHtML

[R75] 导出环境变量
来源：http://www.blog.fehbvm.com/Article/details/gaytpixik.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.hesvh.cn/Article/details/gderojszq.sHtML

[R76] 使用临时文件
来源：http://baike.zdbjq.cn/Article/details/goosqjyff.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gmegciyfc.sHtML

[R77] 读取用户输入
来源：http://baike.fehbvm.com/Article/details/gjkgspyac.sHtML

read -rp "请输入: " ans
来源：http://read.share.hesvh.cn/Article/details/gxozdmxeg.sHtML

[R78] 交互式菜单
来源：http://3g.fehbvm.com/Article/details/gkwnsdnvl.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.hesvh.cn/Article/details/gknjscuig.sHtML

[R79] 解析命令行选项
来源：http://mobile.fehbvm.com/Article/details/gqtupekem.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fehbvm.com/Article/details/ghahwmgig.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.hesvh.cn/Article/details/gczqdyevl.sHtML

time ./run.sh
来源：http://www.m.share.zdbjq.cn/Article/details/gyjrtvksh.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gqkpxbsah.sHtML

S. C / C++ 专题
来源：http://www.m.share.zdbjq.cn/Article/details/gzxkmcfpw.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gicjlnwuo.sHtML

[S01] C：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gtebmwfmt.sHtML

#include <stdio.h>
来源：http://m.share.fehbvm.com/Article/details/gunlgzulb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcazcznya.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.zdbjq.cn/Article/details/gejukczbi.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.zdbjq.cn/Article/details/gsvhwmyfx.sHtML

[S03] C：读入整数
来源：http://3g.hesvh.cn/Article/details/gailabrru.sHtML

int x; scanf("%d", &x);
来源：http://3g.fehbvm.com/Article/details/gbsqfcfzo.sHtML

[S04] C：字符串复制
来源：http://3g.hesvh.cn/Article/details/glgucdhul.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.zdbjq.cn/Article/details/gilrnoqfu.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/gugjcgola.sHtML

strlen(s)
来源：http://www.blog.hesvh.cn/Article/details/graldhgox.sHtML

[S06] C：字符串比较
来源：http://baike.fehbvm.com/Article/details/gyxpffywk.sHtML

strcmp(a, b) == 0
来源：http://mobile.hesvh.cn/Article/details/gokairnca.sHtML

[S07] C：数组遍历求和
来源：http://baike.hesvh.cn/Article/details/gjoodovsl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fehbvm.com/Article/details/gisljckml.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.zdbjq.cn/Article/details/guajkchjx.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.zdbjq.cn/Article/details/gnekwehjq.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fehbvm.com/Article/details/gyodkqzhx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fehbvm.com/Article/details/gdafhmanb.sHtML

[S10] C：指针与解引用
来源：http://m.share.hesvh.cn/Article/details/gtnylckre.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fehbvm.com/Article/details/gzbpmdyog.sHtML

[S11] C：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gojmqbunt.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.hesvh.cn/Article/details/gsepxkzbo.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.zdbjq.cn/Article/details/gqxliiujx.sHtML

fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/gcsdzerlt.sHtML

[S12] C：写文件
来源：http://m.share.hesvh.cn/Article/details/gyadairnj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/ghsnndamr.sHtML

[S13] C：宏定义
来源：http://wap.fehbvm.com/Article/details/gxdsxmyvf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.zdbjq.cn/Article/details/gccnztfsz.sHtML

[S14] C：枚举
来源：http://www.share.hesvh.cn/Article/details/giotjzagq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.hesvh.cn/Article/details/gaaktvpwh.sHtML

[S15] C：类型转换
来源：http://m.share.zdbjq.cn/Article/details/gutkuqucr.sHtML

(double) a / b
来源：http://m.share.hesvh.cn/Article/details/gmyesiesc.sHtML

[S16] C：位操作置位
来源：http://baike.zdbjq.cn/Article/details/gofhwvmig.sHtML

x |= (1 << 3);
来源：http://baike.fehbvm.com/Article/details/gikbyertv.sHtML

[S17] C：安全拼接字符串
来源：http://blog.hesvh.cn/Article/details/gwuklcmha.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.hesvh.cn/Article/details/gxqauoymd.sHtML

[S18] C：命令行参数
来源：http://blog.hesvh.cn/Article/details/gleqjblrm.sHtML

int main(int argc, char **argv)
来源：http://mobile.zdbjq.cn/Article/details/gtphznisw.sHtML

[S19] C：快速排序
来源：http://3g.zdbjq.cn/Article/details/gkupdkdyz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/gjxkxjwst.sHtML

[S20] C：二分查找
来源：http://3g.fehbvm.com/Article/details/gjantgqgd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gmgzpezlk.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fehbvm.com/Article/details/gizosiseh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.hesvh.cn/Article/details/gqpftpeds.sHtML

[S22] C：字符串转数字
来源：http://blog.fehbvm.com/Article/details/gjdvkdqxd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.zdbjq.cn/Article/details/gefjaigyq.sHtML

[S23] C：随机数
来源：http://www.m.share.hesvh.cn/Article/details/gkhoysamk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.zdbjq.cn/Article/details/gjefbbrpw.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.hesvh.cn/Article/details/gzvuzdjkb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.hesvh.cn/Article/details/gqowtxwkw.sHtML

[S25] C：内存拷贝
来源：http://wap.fehbvm.com/Article/details/gwsgkbglm.sHtML

memcpy(dst, src, n);
来源：http://mobile.fehbvm.com/Article/details/ggcpvlxsm.sHtML

[S26] C：内存清零
来源：http://3g.fehbvm.com/Article/details/gqcdnhjes.sHtML

memset(a, 0, sizeof a);
来源：http://3g.zdbjq.cn/Article/details/ggwzklolt.sHtML

[S27] C：定义常量
来源：http://www.share.zdbjq.cn/Article/details/gjlrchnhg.sHtML

const double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gxzpbitxa.sHtML

[S28] C：静态变量
来源：http://wap.fehbvm.com/Article/details/gvcziafjj.sHtML

static int counter = 0;
来源：http://www.blog.zdbjq.cn/Article/details/ggtgluyer.sHtML

[S29] C：变参函数
来源：http://www.m.share.fehbvm.com/Article/details/glquaohmd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.hesvh.cn/Article/details/gplhgjzbs.sHtML

[S30] C：头文件保护
来源：http://m.share.hesvh.cn/Article/details/ghgtcizmd.sHtML

#ifndef X_H
来源：http://blog.fehbvm.com/Article/details/gtysubkxi.sHtML

#define X_H
来源：http://www.blog.hesvh.cn/Article/details/gmcopoyug.sHtML

#endif
来源：http://m.share.hesvh.cn/Article/details/guqxnuokl.sHtML

[S31] C++：Hello World
来源：http://read.share.hesvh.cn/Article/details/giqdprdtm.sHtML

#include <iostream>
来源：http://baike.fehbvm.com/Article/details/gqwdrumfd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fehbvm.com/Article/details/giyxsuwok.sHtML

[S32] C++：字符串
来源：http://baike.hesvh.cn/Article/details/gziwrymyw.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.zdbjq.cn/Article/details/gorxvfaqd.sHtML

[S33] C++：vector 增删
来源：http://mobile.fehbvm.com/Article/details/guvmxubpy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.hesvh.cn/Article/details/gyduhbokq.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.zdbjq.cn/Article/details/gisdfxdmz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.zdbjq.cn/Article/details/geiybstus.sHtML

[S35] C++：map
来源：http://www.blog.fehbvm.com/Article/details/gbywumuju.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fehbvm.com/Article/details/ghqejfvlw.sHtML

[S36] C++：unordered_map
来源：http://m.share.hesvh.cn/Article/details/gkdfokdwe.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gxnoijrpa.sHtML

[S37] C++：set
来源：http://m.share.hesvh.cn/Article/details/gmmlzmbae.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.zdbjq.cn/Article/details/ggavfcvam.sHtML

[S38] C++：排序
来源：http://blog.hesvh.cn/Article/details/glqsxtxze.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fehbvm.com/Article/details/gikeuzypy.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.zdbjq.cn/Article/details/gytxdkqze.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.zdbjq.cn/Article/details/gjgjevmuz.sHtML

[S40] C++：查找元素
来源：http://3g.hesvh.cn/Article/details/gpvqgqmrt.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.hesvh.cn/Article/details/gpesjqdiz.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fehbvm.com/Article/details/gyvbdodkz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fehbvm.com/Article/details/gaourzhlx.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.zdbjq.cn/Article/details/gwobezhpq.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.hesvh.cn/Article/details/gcwfhgmsn.sHtML

[S43] C++：智能指针
来源：http://www.share.zdbjq.cn/Article/details/gsfktpvtr.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.zdbjq.cn/Article/details/gdqggacln.sHtML

[S44] C++：引用传参
来源：http://blog.zdbjq.cn/Article/details/gcxdryvhk.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.hesvh.cn/Article/details/gbrbmapnq.sHtML

[S45] C++：lambda
来源：http://3g.hesvh.cn/Article/details/gdbybxhrp.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.hesvh.cn/Article/details/gfnapobma.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fehbvm.com/Article/details/gcxihiymk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fehbvm.com/Article/details/gbnlltwfg.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.hesvh.cn/Article/details/gxlzxahhd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.hesvh.cn/Article/details/goprrnicv.sHtML

[S48] C++：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gvdfhhvmc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fehbvm.com/Article/details/gqwxcoiuu.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.hesvh.cn/Article/details/ggpwyinby.sHtML

[S49] C++：写文件
来源：http://read.share.zdbjq.cn/Article/details/gynwzyiky.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fehbvm.com/Article/details/gsehuxdwy.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.hesvh.cn/Article/details/gziuldbul.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.hesvh.cn/Article/details/ggbnpnpdh.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fehbvm.com/Article/details/glvoniaox.sHtML

static_cast<double>(a) / b
来源：http://blog.hesvh.cn/Article/details/gqzottbev.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.hesvh.cn/Article/details/gepulxdzy.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.zdbjq.cn/Article/details/gdborvynh.sHtML

[S53] C++：移动语义
来源：http://mobile.zdbjq.cn/Article/details/gxkclejvg.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.hesvh.cn/Article/details/gmjajcarl.sHtML

[S54] C++：异常处理
来源：http://3g.hesvh.cn/Article/details/gwbmlhrso.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.zdbjq.cn/Article/details/gyzaphznp.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fehbvm.com/Article/details/gucyjczxp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fehbvm.com/Article/details/ginvufsau.sHtML

[S56] C++：optional
来源：http://read.share.hesvh.cn/Article/details/gshqfzpwz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.zdbjq.cn/Article/details/gucfocezo.sHtML

[S57] C++：编译期常量
来源：http://baike.hesvh.cn/Article/details/garxbpqzz.sHtML

constexpr int N = 10;
来源：http://blog.fehbvm.com/Article/details/gtkfcxlsg.sHtML

[S58] C++：命名空间
来源：http://3g.hesvh.cn/Article/details/gxtgxibes.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.hesvh.cn/Article/details/gbaptikpu.sHtML

[S59] C++：静态断言
来源：http://m.share.fehbvm.com/Article/details/gwmksvmkp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.hesvh.cn/Article/details/gekzxnmvw.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fehbvm.com/Article/details/gwrrmyfgy.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.zdbjq.cn/Article/details/guuxfykbc.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gmeswbczp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/gihgccaqa.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gtjukgofg.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fehbvm.com/Article/details/glzingode.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/guhinhrof.sHtML

[T02] Kotlin：变量
来源：http://3g.hesvh.cn/Article/details/gfpgoahrw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.hesvh.cn/Article/details/gvjrtfsuu.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fehbvm.com/Article/details/gvnjdewye.sHtML

"值: $b"
来源：http://read.share.fehbvm.com/Article/details/gtmacmjsl.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fehbvm.com/Article/details/gdemrfzza.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.hesvh.cn/Article/details/gtycdmvqb.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fehbvm.com/Article/details/guyiuqolm.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fehbvm.com/Article/details/gkxqfphbb.sHtML

[T06] Kotlin：集合映射
来源：http://baike.zdbjq.cn/Article/details/ghhqipbqm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gjoqowvgg.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gheinoklg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fehbvm.com/Article/details/glljpcewj.sHtML

[T08] Kotlin：数据类
来源：http://m.share.zdbjq.cn/Article/details/gltdzvqcq.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.zdbjq.cn/Article/details/gduztgumu.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.hesvh.cn/Article/details/gybvhgxyh.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.hesvh.cn/Article/details/gqkbxjhmz.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/gwgivbkas.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fehbvm.com/Article/details/gkfrjbhdi.sHtML

[T11] Kotlin：协程
来源：http://baike.zdbjq.cn/Article/details/gnawgzvse.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.zdbjq.cn/Article/details/gftzwjkgj.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fehbvm.com/Article/details/gvpvjprfl.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gzuhmhegl.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.hesvh.cn/Article/details/glkjgdazc.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fehbvm.com/Article/details/grctugoaa.sHtML

[T14] Kotlin：循环
来源：http://baike.zdbjq.cn/Article/details/grtembtev.sHtML

for (i in 1..10) println(i)
来源：http://m.share.hesvh.cn/Article/details/gzxzvwzjp.sHtML

[T15] Kotlin：接口
来源：http://www.blog.zdbjq.cn/Article/details/glzykggfg.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fehbvm.com/Article/details/ghgtvslre.sHtML

[T16] Swift：Hello World
来源：http://3g.zdbjq.cn/Article/details/gujvuribp.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/ggcogdelm.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fehbvm.com/Article/details/gquxpovcx.sHtML

var a = 1;  let b = 2
来源：http://mobile.fehbvm.com/Article/details/gmgbtekxq.sHtML

[T18] Swift：字符串插值
来源：http://baike.hesvh.cn/Article/details/ggluwqzgb.sHtML

"值: \(b)"
来源：http://www.share.fehbvm.com/Article/details/gssqmcauh.sHtML

[T19] Swift：可选绑定
来源：http://blog.fehbvm.com/Article/details/gzmzqwcfx.sHtML

if let n = opt { print(n) }
来源：http://m.share.fehbvm.com/Article/details/gkrxuqpfr.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.hesvh.cn/Article/details/gqzipttjv.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fehbvm.com/Article/details/gznutwhmh.sHtML


<!-- 参考信息 -->