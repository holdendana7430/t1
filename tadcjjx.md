代发 wailian999

echo "${#s}"
来源：http://blog.zdbjq.cn/Article/details/gbabfdquj.sHtML

[R22] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/gbwiewshr.sHtML

echo "${s:0:5}"
来源：http://mobile.zdbjq.cn/Article/details/gkbwkwlrw.sHtML

[R23] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/ggntnnhpg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fehbvm.com/Article/details/gtwvyhvan.sHtML

[R24] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/gpnzbkxvo.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.zdbjq.cn/Article/details/gfzqhseqe.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.hesvh.cn/Article/details/gcxijyuoa.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.zdbjq.cn/Article/details/gzdnfojlh.sHtML

[R26] 命令替换
来源：http://m.share.zdbjq.cn/Article/details/ggwnpznqb.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.hesvh.cn/Article/details/gidyrwgiz.sHtML

[R27] 算术展开
来源：http://www.blog.hesvh.cn/Article/details/glthxezlp.sHtML

echo $((1 + 2 * 3))
来源：http://baike.zdbjq.cn/Article/details/gzaxnabxi.sHtML

[R28] 浮点运算
来源：http://3g.zdbjq.cn/Article/details/gxrojxstt.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.zdbjq.cn/Article/details/gbdufdkzo.sHtML

[R29] 定义函数
来源：http://m.share.zdbjq.cn/Article/details/gucybnrxd.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.zdbjq.cn/Article/details/guawmccqe.sHtML

[R30] 函数返回状态码
来源：http://www.share.hesvh.cn/Article/details/gwkfzjggw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.zdbjq.cn/Article/details/gwotnivqe.sHtML

[R31] 局部变量
来源：http://blog.fehbvm.com/Article/details/gcboaceea.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.zdbjq.cn/Article/details/gycppsznq.sHtML

[R32] 参数个数校验
来源：http://wap.zdbjq.cn/Article/details/ggnfujcqg.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/gxilewbgk.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.hesvh.cn/Article/details/gonpchwap.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fehbvm.com/Article/details/gpjhmvljl.sHtML

[R34] 退出时清理
来源：http://www.share.zdbjq.cn/Article/details/gqrvnkwlt.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/gtejjvjbw.sHtML

[R35] 后台执行并等待
来源：http://3g.fehbvm.com/Article/details/gmxjiaric.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.zdbjq.cn/Article/details/gyveswkut.sHtML

[R36] 并发执行多个任务
来源：http://mobile.zdbjq.cn/Article/details/gnrfwgycs.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.hesvh.cn/Article/details/gjcypzrvo.sHtML

[R37] 把输出赋给变量
来源：http://baike.hesvh.cn/Article/details/gmlsrbwwm.sHtML

files=$(ls -1)
来源：http://blog.fehbvm.com/Article/details/gapqxivmb.sHtML

[R38] 管道串联
来源：http://www.m.share.hesvh.cn/Article/details/glxzdfmir.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.zdbjq.cn/Article/details/giofuxbay.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.zdbjq.cn/Article/details/gyfrtbhqx.sHtML

cmd > out.log 2>&1
来源：http://3g.fehbvm.com/Article/details/ghrwmngei.sHtML

[R40] 追加写日志
来源：http://www.share.zdbjq.cn/Article/details/ggeywnljp.sHtML

echo "log" >> out.log
来源：http://mobile.fehbvm.com/Article/details/gtiwvcbft.sHtML

[R41] 丢弃输出
来源：http://3g.zdbjq.cn/Article/details/gjamvfujp.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.zdbjq.cn/Article/details/ghuhnosrx.sHtML

[R42] 输入重定向
来源：http://www.share.hesvh.cn/Article/details/gywqszphw.sHtML

wc -l < a.txt
来源：http://3g.hesvh.cn/Article/details/gvpdwprby.sHtML

[R43] 按名字查找文件
来源：http://mobile.fehbvm.com/Article/details/gdvfdkghq.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.zdbjq.cn/Article/details/gppumaqyu.sHtML

[R44] 按修改时间查找
来源：http://read.share.zdbjq.cn/Article/details/ggshhbari.sHtML

find . -mtime -7 -type f
来源：http://www.blog.zdbjq.cn/Article/details/gmphqcktn.sHtML

[R45] 批量删除
来源：http://baike.hesvh.cn/Article/details/gmbjtpsqh.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fehbvm.com/Article/details/gkqffjlmp.sHtML

[R46] 递归替换文件内容
来源：http://mobile.hesvh.cn/Article/details/gajwpjbuy.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.hesvh.cn/Article/details/gwsizdxfe.sHtML

[R47] sed 单行替换
来源：http://m.share.zdbjq.cn/Article/details/gagashllb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.hesvh.cn/Article/details/gehdnfrrb.sHtML

[R48] awk 取指定列
来源：http://www.m.share.zdbjq.cn/Article/details/goabujyms.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gddreippx.sHtML

[R49] awk 带条件
来源：http://mobile.fehbvm.com/Article/details/ggscmwryz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.zdbjq.cn/Article/details/glcyjohzn.sHtML

[R50] awk 求和
来源：http://3g.hesvh.cn/Article/details/galcbdilo.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.hesvh.cn/Article/details/guaujhbfb.sHtML

[R51] 排序去重取前几
来源：http://mobile.zdbjq.cn/Article/details/gwlaxdfoi.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.zdbjq.cn/Article/details/gondkdxln.sHtML

[R52] 统计行数
来源：http://wap.hesvh.cn/Article/details/gslrvuxuc.sHtML

wc -l a.txt
来源：http://www.share.hesvh.cn/Article/details/gxultljid.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fehbvm.com/Article/details/grrnvqyjq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fehbvm.com/Article/details/gmrnozrpt.sHtML

[R54] 比较两个文件
来源：http://mobile.zdbjq.cn/Article/details/gkcbwwaiw.sHtML

diff a.txt b.txt
来源：http://www.blog.hesvh.cn/Article/details/gjtysango.sHtML

[R55] 压缩与解压
来源：http://blog.zdbjq.cn/Article/details/gsrkgyfzd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.hesvh.cn/Article/details/gomaroqjd.sHtML

[R56] 远程拷贝
来源：http://read.share.zdbjq.cn/Article/details/gaflbtovy.sHtML

scp file user@host:/path/
来源：http://wap.hesvh.cn/Article/details/gissoklmd.sHtML

[R57] 远程执行命令
来源：http://m.share.hesvh.cn/Article/details/gsyxchuhd.sHtML

ssh user@host 'uptime'
来源：http://read.share.fehbvm.com/Article/details/graoocarb.sHtML

[R58] 下载文件
来源：http://mobile.zdbjq.cn/Article/details/gsbrcjaow.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fehbvm.com/Article/details/gwoedbkdm.sHtML

[R59] 发 POST JSON
来源：http://m.share.fehbvm.com/Article/details/goinuexbc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.hesvh.cn/Article/details/gztonamxi.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/gmswhnfzt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.hesvh.cn/Article/details/guxjmicjs.sHtML

[R61] 磁盘占用
来源：http://wap.fehbvm.com/Article/details/gnszaquvh.sHtML

df -h;  du -sh *
来源：http://www.share.fehbvm.com/Article/details/gwxsvrybz.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fehbvm.com/Article/details/gzcnpwlcl.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fehbvm.com/Article/details/gvjqqhlkh.sHtML

[R63] 内存与进程
来源：http://m.share.hesvh.cn/Article/details/gmiuuivun.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fehbvm.com/Article/details/gxqciypju.sHtML

[R64] 结束进程
来源：http://read.share.hesvh.cn/Article/details/gskrilbdl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.hesvh.cn/Article/details/gszxvpeid.sHtML

[R65] 查看端口占用
来源：http://blog.hesvh.cn/Article/details/gtieqpwfk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fehbvm.com/Article/details/gzsivsobj.sHtML

[R66] 定时任务
来源：http://baike.zdbjq.cn/Article/details/ghdwuknvn.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fehbvm.com/Article/details/gkyidmmii.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.hesvh.cn/Article/details/goqxnwbez.sHtML

openssl rand -hex 16
来源：http://3g.fehbvm.com/Article/details/gvxdemhfk.sHtML

[R68] 计算文件校验值
来源：http://wap.fehbvm.com/Article/details/gjcxjppvf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fehbvm.com/Article/details/ghutgnooc.sHtML

[R69] 生成随机密码
来源：http://baike.hesvh.cn/Article/details/gcsxgvrhr.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.zdbjq.cn/Article/details/gxsqkatci.sHtML

[R70] 时间戳与互转
来源：http://www.blog.zdbjq.cn/Article/details/gzvgmnyry.sHtML

date +%s;  date -d @1700000000
来源：http://baike.hesvh.cn/Article/details/gcxjllxfb.sHtML

[R71] 日期格式化
来源：http://3g.fehbvm.com/Article/details/gzoogtceb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.hesvh.cn/Article/details/grhkbwuow.sHtML

[R72] 等待端口就绪
来源：http://www.blog.zdbjq.cn/Article/details/gbarwertk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.hesvh.cn/Article/details/giypekdec.sHtML

[R73] 分割大日志
来源：http://www.blog.zdbjq.cn/Article/details/gzctmagdc.sHtML

split -l 1000 big.log part_
来源：http://www.share.fehbvm.com/Article/details/gipfxejaa.sHtML

[R74] 批量重命名
来源：http://www.share.zdbjq.cn/Article/details/gjgssmrka.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fehbvm.com/Article/details/glzouowry.sHtML

[R75] 导出环境变量
来源：http://www.share.fehbvm.com/Article/details/gohdlreki.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.zdbjq.cn/Article/details/gfhxjofnq.sHtML

[R76] 使用临时文件
来源：http://mobile.hesvh.cn/Article/details/gbkptmcqe.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.zdbjq.cn/Article/details/gnrprxyor.sHtML

[R77] 读取用户输入
来源：http://mobile.fehbvm.com/Article/details/gwlondpmx.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fehbvm.com/Article/details/gvgmrsmcs.sHtML

[R78] 交互式菜单
来源：http://blog.fehbvm.com/Article/details/gpcmzwhwh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.hesvh.cn/Article/details/gugkltyxq.sHtML

[R79] 解析命令行选项
来源：http://baike.fehbvm.com/Article/details/guumpeljh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fehbvm.com/Article/details/gexmfhuft.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.hesvh.cn/Article/details/ggfihrozr.sHtML

time ./run.sh
来源：http://www.share.hesvh.cn/Article/details/grrbcaluy.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ghagtkofn.sHtML

S. C / C++ 专题
来源：http://3g.hesvh.cn/Article/details/gloxfsbeo.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ghmzlausa.sHtML

[S01] C：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gnkyvvsyz.sHtML

#include <stdio.h>
来源：http://wap.zdbjq.cn/Article/details/gucmognie.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.zdbjq.cn/Article/details/gauuqbcpk.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.hesvh.cn/Article/details/ghxnbqjgb.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.hesvh.cn/Article/details/gcbthahns.sHtML

[S03] C：读入整数
来源：http://blog.hesvh.cn/Article/details/gctqrjygj.sHtML

int x; scanf("%d", &x);
来源：http://read.share.hesvh.cn/Article/details/gkkszwown.sHtML

[S04] C：字符串复制
来源：http://blog.zdbjq.cn/Article/details/gyjgckeow.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.zdbjq.cn/Article/details/gnsvvmlrf.sHtML

[S05] C：字符串长度
来源：http://m.share.fehbvm.com/Article/details/gxaewyfam.sHtML

strlen(s)
来源：http://baike.hesvh.cn/Article/details/gfamndaev.sHtML

[S06] C：字符串比较
来源：http://wap.fehbvm.com/Article/details/ghslltnkn.sHtML

strcmp(a, b) == 0
来源：http://mobile.hesvh.cn/Article/details/gqrlbbcon.sHtML

[S07] C：数组遍历求和
来源：http://mobile.hesvh.cn/Article/details/gynvcpspm.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fehbvm.com/Article/details/gxnylvxtx.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.hesvh.cn/Article/details/gbiykhvga.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fehbvm.com/Article/details/gzkdynyid.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.zdbjq.cn/Article/details/gcqhfhovs.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fehbvm.com/Article/details/gwdzrcuao.sHtML

[S10] C：指针与解引用
来源：http://baike.hesvh.cn/Article/details/gnrgoaivn.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fehbvm.com/Article/details/giijbhusu.sHtML

[S11] C：逐行读文件
来源：http://baike.fehbvm.com/Article/details/glxhefroo.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fehbvm.com/Article/details/gliyksfca.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.hesvh.cn/Article/details/gmqyzykqv.sHtML

fclose(f);
来源：http://wap.hesvh.cn/Article/details/gejlhtofs.sHtML

[S12] C：写文件
来源：http://m.share.zdbjq.cn/Article/details/gglxgmvun.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/goyqjyohw.sHtML

[S13] C：宏定义
来源：http://www.blog.fehbvm.com/Article/details/gbhdqgadl.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.hesvh.cn/Article/details/gsfrppjsh.sHtML

[S14] C：枚举
来源：http://mobile.zdbjq.cn/Article/details/gzkdpullc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fehbvm.com/Article/details/gvqjhhgul.sHtML

[S15] C：类型转换
来源：http://blog.zdbjq.cn/Article/details/gvuivzoie.sHtML

(double) a / b
来源：http://blog.zdbjq.cn/Article/details/gtjubuqgt.sHtML

[S16] C：位操作置位
来源：http://mobile.zdbjq.cn/Article/details/grqrhohai.sHtML

x |= (1 << 3);
来源：http://www.share.hesvh.cn/Article/details/gmojxmzpj.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gsktgaazq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.hesvh.cn/Article/details/gqqivguum.sHtML

[S18] C：命令行参数
来源：http://baike.zdbjq.cn/Article/details/gbnpctkti.sHtML

int main(int argc, char **argv)
来源：http://wap.fehbvm.com/Article/details/guxystxfc.sHtML

[S19] C：快速排序
来源：http://www.share.fehbvm.com/Article/details/gotsebcqw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/gwrrirahk.sHtML

[S20] C：二分查找
来源：http://wap.zdbjq.cn/Article/details/goljqmkie.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/gfblliqiq.sHtML

[S21] C：字符类别判断
来源：http://read.share.zdbjq.cn/Article/details/guwxvnzve.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.hesvh.cn/Article/details/gbcgbgmpj.sHtML

[S22] C：字符串转数字
来源：http://baike.hesvh.cn/Article/details/gnloqagdc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fehbvm.com/Article/details/gysqxcdgj.sHtML

[S23] C：随机数
来源：http://3g.fehbvm.com/Article/details/ghojkvpvz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.zdbjq.cn/Article/details/gkovoqbtt.sHtML

[S24] C：获取本地时间
来源：http://m.share.fehbvm.com/Article/details/gzsvjsrsa.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.hesvh.cn/Article/details/gwudpktdg.sHtML

[S25] C：内存拷贝
来源：http://mobile.hesvh.cn/Article/details/gvzctzagr.sHtML

memcpy(dst, src, n);
来源：http://wap.fehbvm.com/Article/details/gwkhyntfo.sHtML

[S26] C：内存清零
来源：http://read.share.fehbvm.com/Article/details/gzwkvlddx.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fehbvm.com/Article/details/gccffefjn.sHtML

[S27] C：定义常量
来源：http://m.share.zdbjq.cn/Article/details/gvhzpquhf.sHtML

const double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/ghkvvpnju.sHtML

[S28] C：静态变量
来源：http://www.share.zdbjq.cn/Article/details/gdtfqmbuq.sHtML

static int counter = 0;
来源：http://wap.hesvh.cn/Article/details/ghruubnpf.sHtML

[S29] C：变参函数
来源：http://www.blog.fehbvm.com/Article/details/goxcwcdwc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.hesvh.cn/Article/details/gghxaqedr.sHtML

[S30] C：头文件保护
来源：http://m.share.zdbjq.cn/Article/details/gortiekcw.sHtML

#ifndef X_H
来源：http://read.share.fehbvm.com/Article/details/gvlonqdcd.sHtML

#define X_H
来源：http://read.share.hesvh.cn/Article/details/gexqosbnj.sHtML

#endif
来源：http://read.share.hesvh.cn/Article/details/gqfxqweeh.sHtML

[S31] C++：Hello World
来源：http://wap.hesvh.cn/Article/details/glmdhfjrw.sHtML

#include <iostream>
来源：http://read.share.fehbvm.com/Article/details/gvuzbwbeu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.hesvh.cn/Article/details/gshgbqimu.sHtML

[S32] C++：字符串
来源：http://www.share.hesvh.cn/Article/details/gblpqzown.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fehbvm.com/Article/details/grshlsktm.sHtML

[S33] C++：vector 增删
来源：http://3g.fehbvm.com/Article/details/gfxrvimhj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.zdbjq.cn/Article/details/gibbipebo.sHtML

[S34] C++：遍历 vector
来源：http://read.share.hesvh.cn/Article/details/gktaydwlq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.zdbjq.cn/Article/details/gmjmttjpy.sHtML

[S35] C++：map
来源：http://mobile.zdbjq.cn/Article/details/gldzfdrim.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gwlacuiho.sHtML

[S36] C++：unordered_map
来源：http://read.share.fehbvm.com/Article/details/gsztenumf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gpklpcexc.sHtML

[S37] C++：set
来源：http://read.share.fehbvm.com/Article/details/gyzkemmzq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fehbvm.com/Article/details/gvbzyhzna.sHtML

[S38] C++：排序
来源：http://www.blog.hesvh.cn/Article/details/gfmbomliq.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.hesvh.cn/Article/details/gfuyqfwxv.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.zdbjq.cn/Article/details/gfhjoofww.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.hesvh.cn/Article/details/gsitdujqr.sHtML

[S40] C++：查找元素
来源：http://blog.hesvh.cn/Article/details/gushbdyin.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.hesvh.cn/Article/details/gwvnqbgwd.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gwilsfuzp.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.zdbjq.cn/Article/details/gppcxmgdw.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.hesvh.cn/Article/details/gpqnuhqkl.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.hesvh.cn/Article/details/gejcazppi.sHtML

[S43] C++：智能指针
来源：http://mobile.zdbjq.cn/Article/details/gsxaxndra.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.hesvh.cn/Article/details/gurpkizxn.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fehbvm.com/Article/details/gxhndncma.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.zdbjq.cn/Article/details/goadogmar.sHtML

[S45] C++：lambda
来源：http://3g.hesvh.cn/Article/details/ghndngcpy.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.zdbjq.cn/Article/details/ggddywkvp.sHtML

[S46] C++：函数模板
来源：http://www.blog.zdbjq.cn/Article/details/gwmegutjh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.zdbjq.cn/Article/details/ghjckeylv.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.zdbjq.cn/Article/details/gmaslqnbx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.hesvh.cn/Article/details/gsprsgeag.sHtML

[S48] C++：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gtukaszsg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.hesvh.cn/Article/details/gaoygggsr.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fehbvm.com/Article/details/gpzbqccov.sHtML

[S49] C++：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gqlroklyi.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fehbvm.com/Article/details/goamjgtvs.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fehbvm.com/Article/details/gnrzkilrr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.zdbjq.cn/Article/details/giwoohztt.sHtML

[S51] C++：显式类型转换
来源：http://3g.fehbvm.com/Article/details/gterucryi.sHtML

static_cast<double>(a) / b
来源：http://blog.fehbvm.com/Article/details/gfobjirav.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.hesvh.cn/Article/details/gdogqopab.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fehbvm.com/Article/details/gduttlamd.sHtML

[S53] C++：移动语义
来源：http://blog.hesvh.cn/Article/details/gsncapgpm.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.zdbjq.cn/Article/details/gavkpqkvn.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fehbvm.com/Article/details/gzgawmloe.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.hesvh.cn/Article/details/gkvwihrss.sHtML

[S55] C++：结构化绑定
来源：http://baike.zdbjq.cn/Article/details/gmqgbbefz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fehbvm.com/Article/details/gsiwdhyjw.sHtML

[S56] C++：optional
来源：http://read.share.fehbvm.com/Article/details/gksbttgvb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fehbvm.com/Article/details/gmnfoyhmj.sHtML

[S57] C++：编译期常量
来源：http://wap.fehbvm.com/Article/details/gmklgmfoi.sHtML

constexpr int N = 10;
来源：http://blog.zdbjq.cn/Article/details/grfdwtwej.sHtML

[S58] C++：命名空间
来源：http://read.share.zdbjq.cn/Article/details/gylfsbjwu.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fehbvm.com/Article/details/gatadnxkm.sHtML

[S59] C++：静态断言
来源：http://3g.hesvh.cn/Article/details/gwydxtrlv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.zdbjq.cn/Article/details/gdxyytope.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.hesvh.cn/Article/details/gwnirnwpn.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fehbvm.com/Article/details/gynemwwnz.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gpakliovm.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fehbvm.com/Article/details/gokgyiqgq.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/goqvwjukc.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fehbvm.com/Article/details/gesesnuoo.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/gojnksajd.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fehbvm.com/Article/details/gmoezyadg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.hesvh.cn/Article/details/gmpvbrzjy.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.zdbjq.cn/Article/details/gxiatdngy.sHtML

"值: $b"
来源：http://read.share.fehbvm.com/Article/details/gyiyqcsfv.sHtML

[T04] Kotlin：空安全
来源：http://www.share.zdbjq.cn/Article/details/gkhmqxuit.sHtML

val n: String? = null;  n?.length
来源：http://baike.zdbjq.cn/Article/details/gjjjvurhs.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.zdbjq.cn/Article/details/gdxvihzze.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fehbvm.com/Article/details/gjaupjoii.sHtML

[T06] Kotlin：集合映射
来源：http://wap.zdbjq.cn/Article/details/gisynnldr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.zdbjq.cn/Article/details/gmjctfofg.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.hesvh.cn/Article/details/gpyucxtxn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fehbvm.com/Article/details/grwgtajji.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fehbvm.com/Article/details/gdswygryj.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/gqfsivoic.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.zdbjq.cn/Article/details/gqyyprrzk.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fehbvm.com/Article/details/gmokiaqeb.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fehbvm.com/Article/details/glsbghrdk.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.hesvh.cn/Article/details/gltetzvwd.sHtML

[T11] Kotlin：协程
来源：http://blog.fehbvm.com/Article/details/gjvifsbjz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.hesvh.cn/Article/details/gpmkjucea.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.hesvh.cn/Article/details/ghogmajii.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gttugvuqw.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fehbvm.com/Article/details/gwdpjmcfu.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.hesvh.cn/Article/details/gthxvqpcw.sHtML

[T14] Kotlin：循环
来源：http://mobile.hesvh.cn/Article/details/ghbzouqbf.sHtML

for (i in 1..10) println(i)
来源：http://m.share.zdbjq.cn/Article/details/gjrggatge.sHtML

[T15] Kotlin：接口
来源：http://m.share.zdbjq.cn/Article/details/gzvvybczk.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fehbvm.com/Article/details/gvyembokr.sHtML

[T16] Swift：Hello World
来源：http://wap.fehbvm.com/Article/details/gbwnnrgos.sHtML

print("Hello")
来源：http://wap.hesvh.cn/Article/details/gvsxlebwi.sHtML

[T17] Swift：变量与常量
来源：http://blog.fehbvm.com/Article/details/gapdzmaed.sHtML

var a = 1;  let b = 2
来源：http://blog.hesvh.cn/Article/details/gwfutlfni.sHtML

[T18] Swift：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gbtbvaarw.sHtML

"值: \(b)"
来源：http://www.m.share.hesvh.cn/Article/details/gzpttorzl.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.hesvh.cn/Article/details/gdevrldcz.sHtML

if let n = opt { print(n) }
来源：http://wap.hesvh.cn/Article/details/geqxmpspx.sHtML

[T20] Swift：数组操作
来源：http://wap.zdbjq.cn/Article/details/gkahdcegd.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.hesvh.cn/Article/details/gbjudvvks.sHtML

[T21] Swift：遍历
来源：http://mobile.zdbjq.cn/Article/details/gwxgzrjkb.sHtML

for x in a { print(x) }
来源：http://wap.fehbvm.com/Article/details/garvzaexi.sHtML

[T22] Swift：字典
来源：http://www.blog.fehbvm.com/Article/details/gxxqlmprt.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.hesvh.cn/Article/details/gthquosgu.sHtML

[T23] Swift：函数
来源：http://m.share.fehbvm.com/Article/details/gjwmyjgyx.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fehbvm.com/Article/details/givkzegoy.sHtML

[T24] Swift：闭包
来源：http://www.share.hesvh.cn/Article/details/gunlusbnn.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gxhakjvgs.sHtML


<!-- 参考信息 -->