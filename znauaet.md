代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.zdbjq.cn/Article/details/ghagnuemp.sHtML

[R30] 函数返回状态码
来源：http://www.share.hesvh.cn/Article/details/gbzdabjhp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.hesvh.cn/Article/details/gtifdavjh.sHtML

[R31] 局部变量
来源：http://www.blog.hesvh.cn/Article/details/goymqeqhw.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.zdbjq.cn/Article/details/gnffeprgp.sHtML

[R32] 参数个数校验
来源：http://www.blog.fehbvm.com/Article/details/golxcdfvh.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/grpfsewma.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fehbvm.com/Article/details/gjgzejavn.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fehbvm.com/Article/details/gljjjauvo.sHtML

[R34] 退出时清理
来源：http://wap.hesvh.cn/Article/details/gczxtmpgu.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.zdbjq.cn/Article/details/gokfyubcy.sHtML

[R35] 后台执行并等待
来源：http://wap.hesvh.cn/Article/details/gvzmucqbv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fehbvm.com/Article/details/gfatrorsg.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.hesvh.cn/Article/details/gkhuyjxop.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.zdbjq.cn/Article/details/ggetsrejn.sHtML

[R37] 把输出赋给变量
来源：http://wap.hesvh.cn/Article/details/ghvbemiip.sHtML

files=$(ls -1)
来源：http://m.share.fehbvm.com/Article/details/gbkistisf.sHtML

[R38] 管道串联
来源：http://blog.hesvh.cn/Article/details/gssusmczl.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.zdbjq.cn/Article/details/gmrstbbxz.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.zdbjq.cn/Article/details/gvpmirfqm.sHtML

cmd > out.log 2>&1
来源：http://read.share.hesvh.cn/Article/details/gfrogoxyt.sHtML

[R40] 追加写日志
来源：http://blog.hesvh.cn/Article/details/gorfszhyl.sHtML

echo "log" >> out.log
来源：http://www.blog.fehbvm.com/Article/details/grkxystev.sHtML

[R41] 丢弃输出
来源：http://www.share.hesvh.cn/Article/details/gmbswxzaj.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.hesvh.cn/Article/details/gkzfmfpte.sHtML

[R42] 输入重定向
来源：http://www.m.share.fehbvm.com/Article/details/gvexxrafe.sHtML

wc -l < a.txt
来源：http://read.share.zdbjq.cn/Article/details/ghmgtvrqz.sHtML

[R43] 按名字查找文件
来源：http://www.share.hesvh.cn/Article/details/gsdsyqxnb.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.zdbjq.cn/Article/details/gsdejkyaa.sHtML

[R44] 按修改时间查找
来源：http://www.share.fehbvm.com/Article/details/gaeyqwmbs.sHtML

find . -mtime -7 -type f
来源：http://wap.zdbjq.cn/Article/details/gnjzjvopc.sHtML

[R45] 批量删除
来源：http://m.share.fehbvm.com/Article/details/giwbpnczf.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fehbvm.com/Article/details/giymofkpr.sHtML

[R46] 递归替换文件内容
来源：http://wap.hesvh.cn/Article/details/grbuunhlr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.hesvh.cn/Article/details/gxzcifxrb.sHtML

[R47] sed 单行替换
来源：http://blog.fehbvm.com/Article/details/ghrjqzftm.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fehbvm.com/Article/details/glcexqycr.sHtML

[R48] awk 取指定列
来源：http://m.share.hesvh.cn/Article/details/gzqyjdnzy.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fehbvm.com/Article/details/gvfgsybom.sHtML

[R49] awk 带条件
来源：http://www.m.share.zdbjq.cn/Article/details/gtctzhvsj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.hesvh.cn/Article/details/gztrwkifn.sHtML

[R50] awk 求和
来源：http://www.blog.fehbvm.com/Article/details/gntienxvu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fehbvm.com/Article/details/gkryupsha.sHtML

[R51] 排序去重取前几
来源：http://www.blog.zdbjq.cn/Article/details/gwqlscutm.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.zdbjq.cn/Article/details/gcmlybswg.sHtML

[R52] 统计行数
来源：http://www.share.fehbvm.com/Article/details/gersixirv.sHtML

wc -l a.txt
来源：http://mobile.zdbjq.cn/Article/details/gpwwxxuwo.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.zdbjq.cn/Article/details/gugsnhwhi.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fehbvm.com/Article/details/gbdkjgvzo.sHtML

[R54] 比较两个文件
来源：http://www.share.fehbvm.com/Article/details/guxrhygca.sHtML

diff a.txt b.txt
来源：http://m.share.fehbvm.com/Article/details/gcgftligj.sHtML

[R55] 压缩与解压
来源：http://3g.zdbjq.cn/Article/details/gjyiwvlvf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fehbvm.com/Article/details/gqdipjpos.sHtML

[R56] 远程拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gboiiboxn.sHtML

scp file user@host:/path/
来源：http://wap.fehbvm.com/Article/details/gzomrrqgf.sHtML

[R57] 远程执行命令
来源：http://www.blog.zdbjq.cn/Article/details/gwqdydmgh.sHtML

ssh user@host 'uptime'
来源：http://blog.fehbvm.com/Article/details/gxrncewha.sHtML

[R58] 下载文件
来源：http://wap.fehbvm.com/Article/details/gtnzsgdpk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.zdbjq.cn/Article/details/gnlxqoafo.sHtML

[R59] 发 POST JSON
来源：http://mobile.fehbvm.com/Article/details/gvwwzcfot.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fehbvm.com/Article/details/grodladko.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.hesvh.cn/Article/details/gskvogonr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.zdbjq.cn/Article/details/gihahlhwo.sHtML

[R61] 磁盘占用
来源：http://m.share.zdbjq.cn/Article/details/gybjhoxso.sHtML

df -h;  du -sh *
来源：http://blog.zdbjq.cn/Article/details/gnjpesfon.sHtML

[R62] 找最占空间的文件
来源：http://m.share.zdbjq.cn/Article/details/gpbavikfm.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fehbvm.com/Article/details/giuafocsu.sHtML

[R63] 内存与进程
来源：http://www.m.share.zdbjq.cn/Article/details/gcwwcqird.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fehbvm.com/Article/details/guhzjvnmr.sHtML

[R64] 结束进程
来源：http://baike.zdbjq.cn/Article/details/gfwmxvlep.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fehbvm.com/Article/details/gjwniljox.sHtML

[R65] 查看端口占用
来源：http://3g.zdbjq.cn/Article/details/ginsllsic.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.zdbjq.cn/Article/details/gikitgfrm.sHtML

[R66] 定时任务
来源：http://m.share.zdbjq.cn/Article/details/gyxivedyg.sHtML

crontab -e;  crontab -l
来源：http://blog.zdbjq.cn/Article/details/ghemhnsio.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.hesvh.cn/Article/details/girdeluor.sHtML

openssl rand -hex 16
来源：http://mobile.zdbjq.cn/Article/details/gggyhnuur.sHtML

[R68] 计算文件校验值
来源：http://www.share.hesvh.cn/Article/details/grjsdmlld.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.hesvh.cn/Article/details/gqzfnympw.sHtML

[R69] 生成随机密码
来源：http://3g.fehbvm.com/Article/details/gtlisvbfg.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.zdbjq.cn/Article/details/geimavrak.sHtML

[R70] 时间戳与互转
来源：http://baike.hesvh.cn/Article/details/gatwhvfvm.sHtML

date +%s;  date -d @1700000000
来源：http://3g.zdbjq.cn/Article/details/gdzlouryy.sHtML

[R71] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gskcpekdx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.hesvh.cn/Article/details/gldvwalze.sHtML

[R72] 等待端口就绪
来源：http://m.share.hesvh.cn/Article/details/gqoiadaom.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/grfszqenq.sHtML

[R73] 分割大日志
来源：http://m.share.fehbvm.com/Article/details/gmyjpesjf.sHtML

split -l 1000 big.log part_
来源：http://wap.hesvh.cn/Article/details/gafctjzfm.sHtML

[R74] 批量重命名
来源：http://m.share.zdbjq.cn/Article/details/gwmchaayq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.zdbjq.cn/Article/details/ghmmdpjpm.sHtML

[R75] 导出环境变量
来源：http://3g.zdbjq.cn/Article/details/gaqtuskrf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.hesvh.cn/Article/details/gsyukaehg.sHtML

[R76] 使用临时文件
来源：http://www.blog.zdbjq.cn/Article/details/gzsiqacff.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gstijqxcn.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fehbvm.com/Article/details/gtfqgwhnx.sHtML

read -rp "请输入: " ans
来源：http://blog.hesvh.cn/Article/details/gavldgzqz.sHtML

[R78] 交互式菜单
来源：http://baike.hesvh.cn/Article/details/gokevxthy.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.zdbjq.cn/Article/details/ghlatnksh.sHtML

[R79] 解析命令行选项
来源：http://m.share.fehbvm.com/Article/details/gsojuskae.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.zdbjq.cn/Article/details/gvxxcmqay.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.zdbjq.cn/Article/details/gaontohdu.sHtML

time ./run.sh
来源：http://www.blog.fehbvm.com/Article/details/gwvcfwftc.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gzgmshfdf.sHtML

S. C / C++ 专题
来源：http://baike.fehbvm.com/Article/details/gjtuzfpdw.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/grpubznte.sHtML

[S01] C：Hello World
来源：http://read.share.fehbvm.com/Article/details/gqpboplqa.sHtML

#include <stdio.h>
来源：http://read.share.hesvh.cn/Article/details/giddlcwpi.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fehbvm.com/Article/details/gfuuddqoe.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fehbvm.com/Article/details/glfgxpodf.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fehbvm.com/Article/details/gnzhsogkw.sHtML

[S03] C：读入整数
来源：http://blog.fehbvm.com/Article/details/geyqxqgcs.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fehbvm.com/Article/details/gmkzeuufs.sHtML

[S04] C：字符串复制
来源：http://blog.fehbvm.com/Article/details/gawnpswhd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.zdbjq.cn/Article/details/gozutqirr.sHtML

[S05] C：字符串长度
来源：http://wap.zdbjq.cn/Article/details/gopsusaoq.sHtML

strlen(s)
来源：http://blog.hesvh.cn/Article/details/gthykstdt.sHtML

[S06] C：字符串比较
来源：http://m.share.hesvh.cn/Article/details/gqhphqnvx.sHtML

strcmp(a, b) == 0
来源：http://wap.hesvh.cn/Article/details/geowudqge.sHtML

[S07] C：数组遍历求和
来源：http://m.share.hesvh.cn/Article/details/ggozcpots.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fehbvm.com/Article/details/gnllytzls.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fehbvm.com/Article/details/ggtafgvnr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fehbvm.com/Article/details/gscauxvrq.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fehbvm.com/Article/details/gjijukzai.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.zdbjq.cn/Article/details/glibnrpgi.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.hesvh.cn/Article/details/gzvdztjei.sHtML

int *p = &a;  *p = 5;
来源：http://blog.hesvh.cn/Article/details/gazpnynle.sHtML

[S11] C：逐行读文件
来源：http://blog.hesvh.cn/Article/details/goqwfawwn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.zdbjq.cn/Article/details/grzzxevsu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fehbvm.com/Article/details/gsxrauhry.sHtML

fclose(f);
来源：http://mobile.fehbvm.com/Article/details/gxwhmyyzd.sHtML

[S12] C：写文件
来源：http://www.blog.zdbjq.cn/Article/details/gmgnwwoyr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fehbvm.com/Article/details/gjrlkhuqi.sHtML

[S13] C：宏定义
来源：http://m.share.hesvh.cn/Article/details/goohpmdpf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.zdbjq.cn/Article/details/gitnbcisa.sHtML

[S14] C：枚举
来源：http://www.blog.fehbvm.com/Article/details/gpbhtcuzt.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.hesvh.cn/Article/details/gmqrqymhc.sHtML

[S15] C：类型转换
来源：http://3g.zdbjq.cn/Article/details/gdntmzdeo.sHtML

(double) a / b
来源：http://baike.zdbjq.cn/Article/details/gdoockgsm.sHtML

[S16] C：位操作置位
来源：http://read.share.hesvh.cn/Article/details/gxhvkqfxj.sHtML

x |= (1 << 3);
来源：http://blog.fehbvm.com/Article/details/grpgdaxfl.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gnbubidrr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.zdbjq.cn/Article/details/gvjrckeha.sHtML

[S18] C：命令行参数
来源：http://www.blog.hesvh.cn/Article/details/geinfslxp.sHtML

int main(int argc, char **argv)
来源：http://www.blog.zdbjq.cn/Article/details/grnvrwcnc.sHtML

[S19] C：快速排序
来源：http://baike.zdbjq.cn/Article/details/gxrldugmk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/gzsgpwuli.sHtML

[S20] C：二分查找
来源：http://www.blog.fehbvm.com/Article/details/gmhehftxk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/gxupctcar.sHtML

[S21] C：字符类别判断
来源：http://mobile.zdbjq.cn/Article/details/gbppllegd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.zdbjq.cn/Article/details/gexlcazct.sHtML

[S22] C：字符串转数字
来源：http://wap.hesvh.cn/Article/details/gvrijfkjk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.hesvh.cn/Article/details/gtiqhlrhh.sHtML

[S23] C：随机数
来源：http://wap.fehbvm.com/Article/details/gdisvmijw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.hesvh.cn/Article/details/gmixjdhyk.sHtML

[S24] C：获取本地时间
来源：http://www.blog.hesvh.cn/Article/details/gllghjzjq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.hesvh.cn/Article/details/gyheqcjjc.sHtML

[S25] C：内存拷贝
来源：http://www.share.zdbjq.cn/Article/details/glkbaumqb.sHtML

memcpy(dst, src, n);
来源：http://read.share.fehbvm.com/Article/details/gxnckbdwj.sHtML

[S26] C：内存清零
来源：http://www.m.share.zdbjq.cn/Article/details/glvxkqeor.sHtML

memset(a, 0, sizeof a);
来源：http://3g.zdbjq.cn/Article/details/gpjmizaaw.sHtML

[S27] C：定义常量
来源：http://baike.zdbjq.cn/Article/details/gpnfwxpds.sHtML

const double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gdwrwovmt.sHtML

[S28] C：静态变量
来源：http://read.share.zdbjq.cn/Article/details/grxvthsxj.sHtML

static int counter = 0;
来源：http://wap.zdbjq.cn/Article/details/grxuzxiqc.sHtML

[S29] C：变参函数
来源：http://3g.fehbvm.com/Article/details/gkwwpnsmq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.hesvh.cn/Article/details/gwtbjjnov.sHtML

[S30] C：头文件保护
来源：http://www.share.hesvh.cn/Article/details/ggezhxxav.sHtML

#ifndef X_H
来源：http://www.share.hesvh.cn/Article/details/gsvxjywhr.sHtML

#define X_H
来源：http://read.share.zdbjq.cn/Article/details/gzewkfobi.sHtML

#endif
来源：http://wap.zdbjq.cn/Article/details/gznoeavdo.sHtML

[S31] C++：Hello World
来源：http://3g.zdbjq.cn/Article/details/gjmbltopk.sHtML

#include <iostream>
来源：http://read.share.hesvh.cn/Article/details/gydrsqaba.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fehbvm.com/Article/details/gcpaolopv.sHtML

[S32] C++：字符串
来源：http://blog.fehbvm.com/Article/details/gelyjaubx.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.hesvh.cn/Article/details/gvxuczbdf.sHtML

[S33] C++：vector 增删
来源：http://www.blog.zdbjq.cn/Article/details/gqolueslu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.zdbjq.cn/Article/details/givjktraf.sHtML

[S34] C++：遍历 vector
来源：http://blog.zdbjq.cn/Article/details/ghqthmimc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.zdbjq.cn/Article/details/gybkowztx.sHtML

[S35] C++：map
来源：http://read.share.hesvh.cn/Article/details/gvlmbqtjo.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fehbvm.com/Article/details/grloffdhk.sHtML

[S36] C++：unordered_map
来源：http://www.blog.hesvh.cn/Article/details/gmiiiaxeg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/gefubrhdv.sHtML

[S37] C++：set
来源：http://www.blog.hesvh.cn/Article/details/gwgditiqg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.hesvh.cn/Article/details/gyzumoaaz.sHtML

[S38] C++：排序
来源：http://mobile.hesvh.cn/Article/details/gqyvryydn.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.zdbjq.cn/Article/details/gibhdjukw.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.zdbjq.cn/Article/details/gqtuvtiys.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.hesvh.cn/Article/details/gkjravxtx.sHtML

[S40] C++：查找元素
来源：http://www.m.share.hesvh.cn/Article/details/gpdkkmmhn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fehbvm.com/Article/details/gnxdmekpc.sHtML

[S41] C++：类与构造函数
来源：http://blog.fehbvm.com/Article/details/ggqkvyqeb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fehbvm.com/Article/details/gsrcnizdp.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fehbvm.com/Article/details/gnucjfmir.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fehbvm.com/Article/details/gdrmdlans.sHtML

[S43] C++：智能指针
来源：http://www.blog.fehbvm.com/Article/details/gdplmvsqz.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fehbvm.com/Article/details/gixvkalnl.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fehbvm.com/Article/details/gjapvskfu.sHtML

void inc(int &x) { ++x; }
来源：http://3g.zdbjq.cn/Article/details/gibxehenq.sHtML

[S45] C++：lambda
来源：http://3g.fehbvm.com/Article/details/gwyiquxec.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.hesvh.cn/Article/details/gsnsjndug.sHtML

[S46] C++：函数模板
来源：http://www.m.share.hesvh.cn/Article/details/gpjfremfx.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.zdbjq.cn/Article/details/gmkdedugw.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fehbvm.com/Article/details/gynycpoyp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fehbvm.com/Article/details/gfhmdqwur.sHtML

[S48] C++：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gitslnois.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.zdbjq.cn/Article/details/gqzyweeky.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.hesvh.cn/Article/details/gincodrwi.sHtML

[S49] C++：写文件
来源：http://wap.fehbvm.com/Article/details/gjnqxekql.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.zdbjq.cn/Article/details/guyumimad.sHtML

[S50] C++：格式化数字
来源：http://www.blog.zdbjq.cn/Article/details/gxaykobmt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gsdhudwje.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gwqwbneaj.sHtML

static_cast<double>(a) / b
来源：http://mobile.zdbjq.cn/Article/details/gpmqthqcz.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.zdbjq.cn/Article/details/gwcsulktb.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fehbvm.com/Article/details/grbnzwysy.sHtML

[S53] C++：移动语义
来源：http://baike.hesvh.cn/Article/details/ggvrvykto.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.zdbjq.cn/Article/details/gvfjvvbzh.sHtML

[S54] C++：异常处理
来源：http://read.share.zdbjq.cn/Article/details/gbbxbjpnr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fehbvm.com/Article/details/gfzhgysps.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.zdbjq.cn/Article/details/gpkhocwhl.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.zdbjq.cn/Article/details/gpbmoexpr.sHtML

[S56] C++：optional
来源：http://3g.fehbvm.com/Article/details/gifwbxfkq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.zdbjq.cn/Article/details/gnlomffom.sHtML

[S57] C++：编译期常量
来源：http://baike.hesvh.cn/Article/details/ghvwvwtdo.sHtML

constexpr int N = 10;
来源：http://read.share.fehbvm.com/Article/details/gqfihywyf.sHtML

[S58] C++：命名空间
来源：http://blog.fehbvm.com/Article/details/gpnhfngfx.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.zdbjq.cn/Article/details/gpbzqasnp.sHtML

[S59] C++：静态断言
来源：http://mobile.zdbjq.cn/Article/details/gjmedsbwm.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.zdbjq.cn/Article/details/gnlaypnit.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.zdbjq.cn/Article/details/giwkedghj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.zdbjq.cn/Article/details/grvxavaml.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gwhnbewcb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fehbvm.com/Article/details/gwbfcagzi.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gjkvnayae.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gvruffllf.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gwtyefajt.sHtML

[T02] Kotlin：变量
来源：http://3g.hesvh.cn/Article/details/gnhgtddoq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.hesvh.cn/Article/details/gcjsdjftt.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.zdbjq.cn/Article/details/gopizhfiy.sHtML

"值: $b"
来源：http://www.blog.hesvh.cn/Article/details/gdecwfwzf.sHtML

[T04] Kotlin：空安全
来源：http://wap.zdbjq.cn/Article/details/gyapdsbyp.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fehbvm.com/Article/details/gbbeahhkm.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.hesvh.cn/Article/details/gfgnyjebp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fehbvm.com/Article/details/gjofrtzyj.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/gupxjmgoh.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.zdbjq.cn/Article/details/giaupcmrw.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fehbvm.com/Article/details/groiyszqd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fehbvm.com/Article/details/gzgiswdux.sHtML

[T08] Kotlin：数据类
来源：http://3g.zdbjq.cn/Article/details/gpuhcpjts.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fehbvm.com/Article/details/gficyqztp.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.hesvh.cn/Article/details/gmajwkvks.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.hesvh.cn/Article/details/gwhujrdbn.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fehbvm.com/Article/details/ggdrwwfce.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.zdbjq.cn/Article/details/gxqoeinos.sHtML

[T11] Kotlin：协程
来源：http://m.share.fehbvm.com/Article/details/ghgkscxvr.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fehbvm.com/Article/details/gqitabksg.sHtML

[T12] Kotlin：解构声明
来源：http://3g.hesvh.cn/Article/details/ggtvjxvsl.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/ggnntigik.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.zdbjq.cn/Article/details/gvkqrtrro.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.hesvh.cn/Article/details/gljerzrde.sHtML

[T14] Kotlin：循环
来源：http://baike.fehbvm.com/Article/details/grujipsur.sHtML

for (i in 1..10) println(i)
来源：http://wap.zdbjq.cn/Article/details/gwbnlaolj.sHtML

[T15] Kotlin：接口
来源：http://baike.fehbvm.com/Article/details/gytqeamoi.sHtML

interface Shape { fun area(): Double }
来源：http://blog.hesvh.cn/Article/details/guvwsusun.sHtML

[T16] Swift：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gzhjuaxwo.sHtML

print("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gzmsgvyhe.sHtML

[T17] Swift：变量与常量
来源：http://3g.fehbvm.com/Article/details/gilvpriyt.sHtML

var a = 1;  let b = 2
来源：http://wap.hesvh.cn/Article/details/gpfeduent.sHtML

[T18] Swift：字符串插值
来源：http://3g.fehbvm.com/Article/details/gbfpvsbhf.sHtML

"值: \(b)"
来源：http://www.blog.hesvh.cn/Article/details/gvlqpnxbp.sHtML

[T19] Swift：可选绑定
来源：http://m.share.hesvh.cn/Article/details/gibjqrxnk.sHtML

if let n = opt { print(n) }
来源：http://mobile.zdbjq.cn/Article/details/ggxsosubh.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.zdbjq.cn/Article/details/gomufdkpd.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fehbvm.com/Article/details/gkwmqwtwq.sHtML

[T21] Swift：遍历
来源：http://wap.hesvh.cn/Article/details/gpidnhtoa.sHtML

for x in a { print(x) }
来源：http://www.share.fehbvm.com/Article/details/gmtddxrlm.sHtML

[T22] Swift：字典
来源：http://blog.zdbjq.cn/Article/details/gpihcsazh.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.hesvh.cn/Article/details/glyhkilen.sHtML

[T23] Swift：函数
来源：http://mobile.zdbjq.cn/Article/details/galwwyjok.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.zdbjq.cn/Article/details/gdhnqhplw.sHtML

[T24] Swift：闭包
来源：http://wap.zdbjq.cn/Article/details/goamurfvu.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.hesvh.cn/Article/details/gbhihkvmc.sHtML

[T25] Swift：结构体
来源：http://m.share.hesvh.cn/Article/details/gsygenczd.sHtML

struct P { var x: Int }
来源：http://www.share.hesvh.cn/Article/details/geewnwswy.sHtML

[T26] Swift：类与重写
来源：http://m.share.fehbvm.com/Article/details/gvzfhkzkc.sHtML

class A: Base { override func f() {} }
来源：http://baike.fehbvm.com/Article/details/gfiycnntj.sHtML

[T27] Swift：错误处理
来源：http://read.share.hesvh.cn/Article/details/gyosshdeq.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.hesvh.cn/Article/details/gkygnkzdn.sHtML

[T28] Swift：枚举
来源：http://m.share.hesvh.cn/Article/details/goaopwhvw.sHtML

enum Color { case red, green }
来源：http://3g.hesvh.cn/Article/details/gtxgvjvke.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.zdbjq.cn/Article/details/gftjiwpsf.sHtML

guard let x = opt else { return }
来源：http://wap.hesvh.cn/Article/details/geeotqegj.sHtML

[T30] Swift：协议
来源：http://blog.fehbvm.com/Article/details/giqdikfyk.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.hesvh.cn/Article/details/ghrqupknv.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gohcrpusp.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gjaawzvop.sHtML

[T32] Lua：局部变量
来源：http://wap.zdbjq.cn/Article/details/gzigrbfaj.sHtML

local a = 1
来源：http://www.blog.zdbjq.cn/Article/details/grfxrqgod.sHtML


<!-- 参考信息 -->