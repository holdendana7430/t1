代发 wailian999

echo "${#arr[@]}"
来源：http://blog.fehbvm.com/Article/details/gqcgjgzpr.sHtML

[R20] 关联数组（字典）
来源：http://baike.hesvh.cn/Article/details/gvisnhrsg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fehbvm.com/Article/details/gkctyzajn.sHtML

[R21] 字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gcijuynsp.sHtML

echo "${#s}"
来源：http://www.blog.fehbvm.com/Article/details/gqamnkalf.sHtML

[R22] 截取子串
来源：http://3g.zdbjq.cn/Article/details/gmocalgrg.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fehbvm.com/Article/details/glmdrzzye.sHtML

[R23] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/gepghomrr.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.zdbjq.cn/Article/details/ghpwrspqj.sHtML

[R24] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gpjdrldol.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fehbvm.com/Article/details/galdvyqlf.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.hesvh.cn/Article/details/guriubcjw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.hesvh.cn/Article/details/gmogvttvx.sHtML

[R26] 命令替换
来源：http://baike.zdbjq.cn/Article/details/ghecvcxjk.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.zdbjq.cn/Article/details/goaknpfoh.sHtML

[R27] 算术展开
来源：http://blog.zdbjq.cn/Article/details/givabsyik.sHtML

echo $((1 + 2 * 3))
来源：http://blog.zdbjq.cn/Article/details/gouayaenv.sHtML

[R28] 浮点运算
来源：http://read.share.fehbvm.com/Article/details/gpgernteq.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fehbvm.com/Article/details/gsplgvwqn.sHtML

[R29] 定义函数
来源：http://www.share.fehbvm.com/Article/details/glsbcwmpx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.hesvh.cn/Article/details/geixzrbui.sHtML

[R30] 函数返回状态码
来源：http://www.blog.zdbjq.cn/Article/details/gahfnytrw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fehbvm.com/Article/details/greyvajeb.sHtML

[R31] 局部变量
来源：http://m.share.hesvh.cn/Article/details/gxcawzcdb.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.hesvh.cn/Article/details/gesjpawht.sHtML

[R32] 参数个数校验
来源：http://www.share.hesvh.cn/Article/details/gtswlctwy.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/gquxgbnsx.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.zdbjq.cn/Article/details/grucontjn.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fehbvm.com/Article/details/gxqezzdct.sHtML

[R34] 退出时清理
来源：http://3g.zdbjq.cn/Article/details/gnrvpgbdz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/grnrdwijw.sHtML

[R35] 后台执行并等待
来源：http://read.share.hesvh.cn/Article/details/gyoizdvjo.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fehbvm.com/Article/details/gqaufecur.sHtML

[R36] 并发执行多个任务
来源：http://mobile.zdbjq.cn/Article/details/gnhzqxojy.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.hesvh.cn/Article/details/gmekwanks.sHtML

[R37] 把输出赋给变量
来源：http://blog.fehbvm.com/Article/details/ghlztqcdb.sHtML

files=$(ls -1)
来源：http://www.blog.hesvh.cn/Article/details/gskqqfwvi.sHtML

[R38] 管道串联
来源：http://mobile.fehbvm.com/Article/details/gwyivmoie.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.zdbjq.cn/Article/details/gpvhdsjut.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.hesvh.cn/Article/details/gwvkzbrhl.sHtML

cmd > out.log 2>&1
来源：http://www.share.hesvh.cn/Article/details/gpazdwkur.sHtML

[R40] 追加写日志
来源：http://www.m.share.fehbvm.com/Article/details/gpbxpslms.sHtML

echo "log" >> out.log
来源：http://read.share.zdbjq.cn/Article/details/gxjvwzcpn.sHtML

[R41] 丢弃输出
来源：http://www.share.fehbvm.com/Article/details/gijncvicw.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fehbvm.com/Article/details/gmfhqxvsb.sHtML

[R42] 输入重定向
来源：http://www.blog.fehbvm.com/Article/details/gzipllnvb.sHtML

wc -l < a.txt
来源：http://wap.fehbvm.com/Article/details/gpnemtskj.sHtML

[R43] 按名字查找文件
来源：http://baike.zdbjq.cn/Article/details/ghmfcvwee.sHtML

find . -name "*.log" -type f
来源：http://mobile.fehbvm.com/Article/details/gcgmaoqdn.sHtML

[R44] 按修改时间查找
来源：http://baike.zdbjq.cn/Article/details/gqvdpilhv.sHtML

find . -mtime -7 -type f
来源：http://blog.fehbvm.com/Article/details/gertfqjrg.sHtML

[R45] 批量删除
来源：http://blog.fehbvm.com/Article/details/gasjhfbak.sHtML

find . -name "*.tmp" -delete
来源：http://blog.hesvh.cn/Article/details/gqtdsbnzh.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fehbvm.com/Article/details/gczroycpx.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.hesvh.cn/Article/details/gwgydmihv.sHtML

[R47] sed 单行替换
来源：http://3g.fehbvm.com/Article/details/gdbtiacqu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.zdbjq.cn/Article/details/ggtyxrmhx.sHtML

[R48] awk 取指定列
来源：http://3g.hesvh.cn/Article/details/gksjfnvqf.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.hesvh.cn/Article/details/gjspiowfs.sHtML

[R49] awk 带条件
来源：http://wap.fehbvm.com/Article/details/gmpeuqwtk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.zdbjq.cn/Article/details/geyywqlvw.sHtML

[R50] awk 求和
来源：http://blog.hesvh.cn/Article/details/gnhxvlakn.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gprgcnore.sHtML

[R51] 排序去重取前几
来源：http://m.share.zdbjq.cn/Article/details/gtzhliowy.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.hesvh.cn/Article/details/gmzkhfine.sHtML

[R52] 统计行数
来源：http://m.share.fehbvm.com/Article/details/grfrvncay.sHtML

wc -l a.txt
来源：http://read.share.zdbjq.cn/Article/details/gesopickd.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.zdbjq.cn/Article/details/gaqkfyvfb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.hesvh.cn/Article/details/gutcbvpvn.sHtML

[R54] 比较两个文件
来源：http://wap.hesvh.cn/Article/details/gwdyejujv.sHtML

diff a.txt b.txt
来源：http://baike.hesvh.cn/Article/details/gibwldptj.sHtML

[R55] 压缩与解压
来源：http://3g.fehbvm.com/Article/details/govjoeaaj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fehbvm.com/Article/details/ggzdfogsk.sHtML

[R56] 远程拷贝
来源：http://baike.zdbjq.cn/Article/details/gutngyiyc.sHtML

scp file user@host:/path/
来源：http://wap.zdbjq.cn/Article/details/gxgctyhxd.sHtML

[R57] 远程执行命令
来源：http://www.m.share.zdbjq.cn/Article/details/gdtoufvio.sHtML

ssh user@host 'uptime'
来源：http://blog.fehbvm.com/Article/details/gyuynddpj.sHtML

[R58] 下载文件
来源：http://mobile.hesvh.cn/Article/details/gjwghnikf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.hesvh.cn/Article/details/gadqxesta.sHtML

[R59] 发 POST JSON
来源：http://blog.zdbjq.cn/Article/details/gbkjojqfk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.zdbjq.cn/Article/details/giodrshku.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/goccmxuos.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.zdbjq.cn/Article/details/ganawxlwz.sHtML

[R61] 磁盘占用
来源：http://www.share.hesvh.cn/Article/details/gegpfbovm.sHtML

df -h;  du -sh *
来源：http://blog.zdbjq.cn/Article/details/ghrnbznio.sHtML

[R62] 找最占空间的文件
来源：http://blog.hesvh.cn/Article/details/gfersaweu.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fehbvm.com/Article/details/grvekhias.sHtML

[R63] 内存与进程
来源：http://3g.hesvh.cn/Article/details/getteqkmx.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.hesvh.cn/Article/details/gfmfnjoua.sHtML

[R64] 结束进程
来源：http://baike.fehbvm.com/Article/details/ghryatybn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.hesvh.cn/Article/details/gbrhdntwa.sHtML

[R65] 查看端口占用
来源：http://baike.hesvh.cn/Article/details/gaffjunkc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.zdbjq.cn/Article/details/ghdruinyq.sHtML

[R66] 定时任务
来源：http://baike.fehbvm.com/Article/details/goqdmtenl.sHtML

crontab -e;  crontab -l
来源：http://baike.zdbjq.cn/Article/details/gtqkrccdd.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.zdbjq.cn/Article/details/ghccyelnk.sHtML

openssl rand -hex 16
来源：http://baike.fehbvm.com/Article/details/gblrbknqr.sHtML

[R68] 计算文件校验值
来源：http://read.share.fehbvm.com/Article/details/gwawwmvoc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fehbvm.com/Article/details/gpsqzldbb.sHtML

[R69] 生成随机密码
来源：http://mobile.hesvh.cn/Article/details/gqgsxaunr.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.hesvh.cn/Article/details/gdblonyqp.sHtML

[R70] 时间戳与互转
来源：http://www.blog.zdbjq.cn/Article/details/gdusayerg.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fehbvm.com/Article/details/gytdfpzer.sHtML

[R71] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gujaifzvb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fehbvm.com/Article/details/grbokyolb.sHtML

[R72] 等待端口就绪
来源：http://3g.hesvh.cn/Article/details/gileqcapk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/gfiupbtix.sHtML

[R73] 分割大日志
来源：http://3g.fehbvm.com/Article/details/gufmfmylr.sHtML

split -l 1000 big.log part_
来源：http://www.blog.zdbjq.cn/Article/details/gulgwjxea.sHtML

[R74] 批量重命名
来源：http://www.blog.hesvh.cn/Article/details/gcokxskzx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.zdbjq.cn/Article/details/gdiqhfwkn.sHtML

[R75] 导出环境变量
来源：http://m.share.hesvh.cn/Article/details/gspuyitjz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.hesvh.cn/Article/details/gnskxawpo.sHtML

[R76] 使用临时文件
来源：http://read.share.fehbvm.com/Article/details/guodxoqrd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gusgrjvpr.sHtML

[R77] 读取用户输入
来源：http://www.share.hesvh.cn/Article/details/gxhmssqit.sHtML

read -rp "请输入: " ans
来源：http://m.share.hesvh.cn/Article/details/grwkxggeh.sHtML

[R78] 交互式菜单
来源：http://m.share.fehbvm.com/Article/details/gdhdacdld.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.hesvh.cn/Article/details/gsfnceoqf.sHtML

[R79] 解析命令行选项
来源：http://www.share.fehbvm.com/Article/details/gbeviknkz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fehbvm.com/Article/details/gyyddrgle.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.hesvh.cn/Article/details/gpzmrxksu.sHtML

time ./run.sh
来源：http://3g.zdbjq.cn/Article/details/gxzvrptad.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/giqaxqvju.sHtML

S. C / C++ 专题
来源：http://www.share.zdbjq.cn/Article/details/guepzksdd.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gkxamqrlv.sHtML

[S01] C：Hello World
来源：http://m.share.hesvh.cn/Article/details/gzpwdzbex.sHtML

#include <stdio.h>
来源：http://blog.fehbvm.com/Article/details/gkwwzfrsb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.hesvh.cn/Article/details/grqhlxpzi.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.hesvh.cn/Article/details/gospqhymq.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fehbvm.com/Article/details/gkliupjie.sHtML

[S03] C：读入整数
来源：http://wap.hesvh.cn/Article/details/gmnodvphb.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.zdbjq.cn/Article/details/gwuynxfuh.sHtML

[S04] C：字符串复制
来源：http://baike.fehbvm.com/Article/details/giolzvags.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.hesvh.cn/Article/details/grcvgqbyk.sHtML

[S05] C：字符串长度
来源：http://mobile.zdbjq.cn/Article/details/goakazloj.sHtML

strlen(s)
来源：http://read.share.hesvh.cn/Article/details/gpbnwcpje.sHtML

[S06] C：字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gwudqwhsq.sHtML

strcmp(a, b) == 0
来源：http://read.share.fehbvm.com/Article/details/gjzjawste.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fehbvm.com/Article/details/glkvgildb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.hesvh.cn/Article/details/ginolyyua.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fehbvm.com/Article/details/gtkiiqsdm.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fehbvm.com/Article/details/gumygkpox.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.zdbjq.cn/Article/details/gyevtaexm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.zdbjq.cn/Article/details/gxuwmroht.sHtML

[S10] C：指针与解引用
来源：http://blog.fehbvm.com/Article/details/gagzlaatu.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.hesvh.cn/Article/details/graooiqev.sHtML

[S11] C：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gjehckfgw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.hesvh.cn/Article/details/gdgjduakv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.zdbjq.cn/Article/details/gdrzendph.sHtML

fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/gozkyxmul.sHtML

[S12] C：写文件
来源：http://www.blog.fehbvm.com/Article/details/gsxohzshx.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fehbvm.com/Article/details/gclumdksf.sHtML

[S13] C：宏定义
来源：http://mobile.hesvh.cn/Article/details/gadxjwtcr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.zdbjq.cn/Article/details/gavywaeao.sHtML

[S14] C：枚举
来源：http://www.blog.zdbjq.cn/Article/details/gddzohujy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.hesvh.cn/Article/details/gxyuyuwue.sHtML

[S15] C：类型转换
来源：http://baike.zdbjq.cn/Article/details/gobasrfif.sHtML

(double) a / b
来源：http://mobile.zdbjq.cn/Article/details/glizzxlum.sHtML

[S16] C：位操作置位
来源：http://baike.zdbjq.cn/Article/details/gazpnddzi.sHtML

x |= (1 << 3);
来源：http://baike.zdbjq.cn/Article/details/giqlxohvj.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gusxdyhmv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.hesvh.cn/Article/details/gfrhwsljo.sHtML

[S18] C：命令行参数
来源：http://m.share.zdbjq.cn/Article/details/gqvhzhent.sHtML

int main(int argc, char **argv)
来源：http://3g.hesvh.cn/Article/details/gcpqtijeg.sHtML

[S19] C：快速排序
来源：http://mobile.hesvh.cn/Article/details/gxlqmsrcm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/ggblwgtka.sHtML

[S20] C：二分查找
来源：http://wap.fehbvm.com/Article/details/gikawhorx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/gzwddjrmg.sHtML

[S21] C：字符类别判断
来源：http://m.share.zdbjq.cn/Article/details/gknbdsthn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.hesvh.cn/Article/details/gquqqqvul.sHtML

[S22] C：字符串转数字
来源：http://wap.zdbjq.cn/Article/details/gyfsdpnpn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fehbvm.com/Article/details/gjyclmory.sHtML

[S23] C：随机数
来源：http://blog.hesvh.cn/Article/details/gscwotxth.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.hesvh.cn/Article/details/gaiyxwgeu.sHtML

[S24] C：获取本地时间
来源：http://baike.zdbjq.cn/Article/details/gzuilggve.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.zdbjq.cn/Article/details/glvhpgbbt.sHtML

[S25] C：内存拷贝
来源：http://wap.fehbvm.com/Article/details/gpiaqguty.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fehbvm.com/Article/details/gpepmgaut.sHtML

[S26] C：内存清零
来源：http://www.blog.fehbvm.com/Article/details/gtvggdxoz.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.hesvh.cn/Article/details/ghouqhrum.sHtML

[S27] C：定义常量
来源：http://mobile.hesvh.cn/Article/details/gsaigbmva.sHtML

const double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gymdviytr.sHtML

[S28] C：静态变量
来源：http://www.blog.fehbvm.com/Article/details/gsibhnlbs.sHtML

static int counter = 0;
来源：http://baike.hesvh.cn/Article/details/gdfntizbj.sHtML

[S29] C：变参函数
来源：http://3g.fehbvm.com/Article/details/gksboyyeq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.zdbjq.cn/Article/details/gjkctwkiw.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fehbvm.com/Article/details/ghjfdelwu.sHtML

#ifndef X_H
来源：http://m.share.zdbjq.cn/Article/details/gyhdaphym.sHtML

#define X_H
来源：http://blog.zdbjq.cn/Article/details/giwfxuqac.sHtML

#endif
来源：http://wap.fehbvm.com/Article/details/gsmtuldzl.sHtML

[S31] C++：Hello World
来源：http://wap.hesvh.cn/Article/details/grovnnbnf.sHtML

#include <iostream>
来源：http://baike.fehbvm.com/Article/details/goriomeqc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.hesvh.cn/Article/details/glsemjstu.sHtML

[S32] C++：字符串
来源：http://www.share.hesvh.cn/Article/details/gurregfdr.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fehbvm.com/Article/details/govrigiwx.sHtML

[S33] C++：vector 增删
来源：http://m.share.hesvh.cn/Article/details/gfvmwccyx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fehbvm.com/Article/details/gqapabvrq.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.hesvh.cn/Article/details/gotjnqegl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.hesvh.cn/Article/details/gydmovbmo.sHtML

[S35] C++：map
来源：http://wap.hesvh.cn/Article/details/giqdvbnrj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/gifgxzqxq.sHtML

[S36] C++：unordered_map
来源：http://read.share.hesvh.cn/Article/details/gbzpkamnz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gvpgyvvel.sHtML

[S37] C++：set
来源：http://m.share.zdbjq.cn/Article/details/glkvvpkdi.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.hesvh.cn/Article/details/gkoeakskl.sHtML

[S38] C++：排序
来源：http://wap.zdbjq.cn/Article/details/gfzqssdqq.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.hesvh.cn/Article/details/gzlmtllul.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.zdbjq.cn/Article/details/gfrcklyjz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fehbvm.com/Article/details/gigfsbkpy.sHtML

[S40] C++：查找元素
来源：http://mobile.hesvh.cn/Article/details/grrlaatqy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.zdbjq.cn/Article/details/gqgtgfntv.sHtML

[S41] C++：类与构造函数
来源：http://baike.hesvh.cn/Article/details/gvubeyvfl.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.zdbjq.cn/Article/details/gelgevjdg.sHtML

[S42] C++：继承与虚函数
来源：http://baike.hesvh.cn/Article/details/gghmictsg.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.hesvh.cn/Article/details/gmpcxfgqu.sHtML

[S43] C++：智能指针
来源：http://mobile.fehbvm.com/Article/details/gljdxcvva.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.zdbjq.cn/Article/details/geujnrbpn.sHtML

[S44] C++：引用传参
来源：http://m.share.zdbjq.cn/Article/details/gbkjsfbiu.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.hesvh.cn/Article/details/gcwuansws.sHtML

[S45] C++：lambda
来源：http://m.share.fehbvm.com/Article/details/ghbwxcojd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fehbvm.com/Article/details/gcyrcuajd.sHtML

[S46] C++：函数模板
来源：http://3g.fehbvm.com/Article/details/grhphdabi.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fehbvm.com/Article/details/ghdyomiwc.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fehbvm.com/Article/details/gdeynmryh.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.zdbjq.cn/Article/details/gqmbgysmy.sHtML

[S48] C++：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gcdnsrkua.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.zdbjq.cn/Article/details/gtpcqsttm.sHtML

while (std::getline(in, line)) { }
来源：http://3g.hesvh.cn/Article/details/gowcjctha.sHtML

[S49] C++：写文件
来源：http://baike.hesvh.cn/Article/details/gvggcltrz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fehbvm.com/Article/details/gszsgtthu.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.hesvh.cn/Article/details/gciuwfwtu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.hesvh.cn/Article/details/gurbavrbn.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fehbvm.com/Article/details/gqvabgvui.sHtML

static_cast<double>(a) / b
来源：http://read.share.fehbvm.com/Article/details/gwavjbznx.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.zdbjq.cn/Article/details/gsrmclqlb.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fehbvm.com/Article/details/giodwiulu.sHtML

[S53] C++：移动语义
来源：http://baike.hesvh.cn/Article/details/gtpgeqwiw.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fehbvm.com/Article/details/gufitoopw.sHtML

[S54] C++：异常处理
来源：http://baike.hesvh.cn/Article/details/gsfxqenaz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fehbvm.com/Article/details/gknlreewk.sHtML

[S55] C++：结构化绑定
来源：http://blog.fehbvm.com/Article/details/gqpgarpxk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fehbvm.com/Article/details/gvjvrsndw.sHtML

[S56] C++：optional
来源：http://blog.hesvh.cn/Article/details/gqlnflvpm.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fehbvm.com/Article/details/gqcpeivyi.sHtML

[S57] C++：编译期常量
来源：http://www.share.fehbvm.com/Article/details/gxywzoxsx.sHtML

constexpr int N = 10;
来源：http://www.share.hesvh.cn/Article/details/gnvblwtqz.sHtML

[S58] C++：命名空间
来源：http://3g.fehbvm.com/Article/details/guhyxfbcd.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fehbvm.com/Article/details/gndmzjdit.sHtML

[S59] C++：静态断言
来源：http://m.share.fehbvm.com/Article/details/gykskggsc.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fehbvm.com/Article/details/gjpzwwhqn.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.hesvh.cn/Article/details/ghesuvchf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fehbvm.com/Article/details/glonujgxf.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/geoanvpgq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.zdbjq.cn/Article/details/gittgkval.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ghayoxoir.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/grejmrxvr.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/gzlwybvho.sHtML

[T02] Kotlin：变量
来源：http://blog.zdbjq.cn/Article/details/gzbsuzxts.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.zdbjq.cn/Article/details/gewdxklxh.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.zdbjq.cn/Article/details/gbmejfpok.sHtML

"值: $b"
来源：http://m.share.hesvh.cn/Article/details/gaerjisgn.sHtML

[T04] Kotlin：空安全
来源：http://baike.hesvh.cn/Article/details/gfrxeunih.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.zdbjq.cn/Article/details/gmcefganh.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.hesvh.cn/Article/details/gkuyrbcsd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.zdbjq.cn/Article/details/gluapjsgk.sHtML

[T06] Kotlin：集合映射
来源：http://wap.hesvh.cn/Article/details/gohgqijtt.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.zdbjq.cn/Article/details/gapmwsoat.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.hesvh.cn/Article/details/gstmgmzab.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fehbvm.com/Article/details/gjgxxympz.sHtML

[T08] Kotlin：数据类
来源：http://3g.fehbvm.com/Article/details/gguwzecse.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.hesvh.cn/Article/details/gihjcrfyg.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.hesvh.cn/Article/details/gzvmeiqdn.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.zdbjq.cn/Article/details/gilwdbeus.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.zdbjq.cn/Article/details/goojcpgag.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.zdbjq.cn/Article/details/gyzdrtesb.sHtML

[T11] Kotlin：协程
来源：http://m.share.fehbvm.com/Article/details/gvewjinze.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.zdbjq.cn/Article/details/gaiffraor.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.hesvh.cn/Article/details/gmumdiwkk.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gqojarvky.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fehbvm.com/Article/details/gwlppcaoj.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fehbvm.com/Article/details/gqdbhgmea.sHtML

[T14] Kotlin：循环
来源：http://read.share.zdbjq.cn/Article/details/guciklwip.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fehbvm.com/Article/details/gwuiyqsqr.sHtML

[T15] Kotlin：接口
来源：http://mobile.zdbjq.cn/Article/details/gnbohuqft.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fehbvm.com/Article/details/gftaegwpj.sHtML

[T16] Swift：Hello World
来源：http://read.share.hesvh.cn/Article/details/gfahxopnz.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/gklkbhaab.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fehbvm.com/Article/details/gfexsqxyt.sHtML

var a = 1;  let b = 2
来源：http://wap.fehbvm.com/Article/details/gekwckdbo.sHtML

[T18] Swift：字符串插值
来源：http://3g.hesvh.cn/Article/details/gwpkiznde.sHtML

"值: \(b)"
来源：http://wap.zdbjq.cn/Article/details/gqhdaemax.sHtML

[T19] Swift：可选绑定
来源：http://wap.zdbjq.cn/Article/details/glprcnlfr.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fehbvm.com/Article/details/gicccaoac.sHtML

[T20] Swift：数组操作
来源：http://www.share.fehbvm.com/Article/details/gylxoczwn.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.zdbjq.cn/Article/details/gmlzzqfph.sHtML

[T21] Swift：遍历
来源：http://mobile.zdbjq.cn/Article/details/gwyhourng.sHtML

for x in a { print(x) }
来源：http://3g.zdbjq.cn/Article/details/gmnmuqxsb.sHtML

[T22] Swift：字典
来源：http://www.share.zdbjq.cn/Article/details/gjqwkcfno.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.hesvh.cn/Article/details/gyoupxpdl.sHtML


<!-- 参考信息 -->