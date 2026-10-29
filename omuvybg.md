代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://blog.zdbjq.cn/Article/details/gyhykinaj.sHtML

[R32] 参数个数校验
来源：http://www.share.zdbjq.cn/Article/details/gybjsdpnc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/gaqodfqbh.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.hesvh.cn/Article/details/gbdmpgfuh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.zdbjq.cn/Article/details/geltftejc.sHtML

[R34] 退出时清理
来源：http://www.m.share.hesvh.cn/Article/details/gffcanupe.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/ghucqfrqf.sHtML

[R35] 后台执行并等待
来源：http://read.share.zdbjq.cn/Article/details/gmulyrfgk.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.hesvh.cn/Article/details/gfjsassgp.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fehbvm.com/Article/details/gzhedinjr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.zdbjq.cn/Article/details/gopijfcxf.sHtML

[R37] 把输出赋给变量
来源：http://baike.hesvh.cn/Article/details/gllpvsvpi.sHtML

files=$(ls -1)
来源：http://3g.fehbvm.com/Article/details/gilspfxlr.sHtML

[R38] 管道串联
来源：http://mobile.fehbvm.com/Article/details/gokzuyxtp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.zdbjq.cn/Article/details/gequmhbgu.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.zdbjq.cn/Article/details/gikuprulz.sHtML

cmd > out.log 2>&1
来源：http://blog.zdbjq.cn/Article/details/gesmyeowt.sHtML

[R40] 追加写日志
来源：http://www.share.fehbvm.com/Article/details/gwaefctez.sHtML

echo "log" >> out.log
来源：http://3g.fehbvm.com/Article/details/ghzqkiyrq.sHtML

[R41] 丢弃输出
来源：http://mobile.zdbjq.cn/Article/details/getmvlldh.sHtML

cmd >/dev/null 2>&1
来源：http://baike.hesvh.cn/Article/details/gzthrxdik.sHtML

[R42] 输入重定向
来源：http://www.m.share.hesvh.cn/Article/details/gtmocoypz.sHtML

wc -l < a.txt
来源：http://3g.zdbjq.cn/Article/details/ggrcgpraf.sHtML

[R43] 按名字查找文件
来源：http://blog.fehbvm.com/Article/details/gnrwedjzb.sHtML

find . -name "*.log" -type f
来源：http://baike.fehbvm.com/Article/details/glizeodqx.sHtML

[R44] 按修改时间查找
来源：http://read.share.fehbvm.com/Article/details/grgfokkjr.sHtML

find . -mtime -7 -type f
来源：http://wap.fehbvm.com/Article/details/gyqwgoxgg.sHtML

[R45] 批量删除
来源：http://blog.zdbjq.cn/Article/details/ggdebbexq.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.hesvh.cn/Article/details/gkenlmjli.sHtML

[R46] 递归替换文件内容
来源：http://mobile.zdbjq.cn/Article/details/gkvzfehxr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.zdbjq.cn/Article/details/gryeqfjeg.sHtML

[R47] sed 单行替换
来源：http://wap.hesvh.cn/Article/details/ghtgbowtj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.hesvh.cn/Article/details/ggxwwprfy.sHtML

[R48] awk 取指定列
来源：http://www.blog.fehbvm.com/Article/details/gxukbwbjs.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fehbvm.com/Article/details/gupdcjwug.sHtML

[R49] awk 带条件
来源：http://blog.hesvh.cn/Article/details/gignqbjgd.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fehbvm.com/Article/details/gjzxhhswk.sHtML

[R50] awk 求和
来源：http://www.share.hesvh.cn/Article/details/gtfkaftzl.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.hesvh.cn/Article/details/gshqbkroq.sHtML

[R51] 排序去重取前几
来源：http://www.blog.zdbjq.cn/Article/details/gtguiqayt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.hesvh.cn/Article/details/gmlznqfml.sHtML

[R52] 统计行数
来源：http://m.share.fehbvm.com/Article/details/gqftwhexm.sHtML

wc -l a.txt
来源：http://www.share.fehbvm.com/Article/details/gruhxfqxz.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.zdbjq.cn/Article/details/geuafqyvp.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fehbvm.com/Article/details/gylblvyfr.sHtML

[R54] 比较两个文件
来源：http://read.share.zdbjq.cn/Article/details/gkniiknbj.sHtML

diff a.txt b.txt
来源：http://m.share.fehbvm.com/Article/details/guayjeixz.sHtML

[R55] 压缩与解压
来源：http://www.m.share.zdbjq.cn/Article/details/ghbkvykka.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.hesvh.cn/Article/details/geeyrlvvv.sHtML

[R56] 远程拷贝
来源：http://blog.fehbvm.com/Article/details/gkgkpueto.sHtML

scp file user@host:/path/
来源：http://mobile.hesvh.cn/Article/details/gorqaxqtz.sHtML

[R57] 远程执行命令
来源：http://www.share.hesvh.cn/Article/details/gtnumjfwa.sHtML

ssh user@host 'uptime'
来源：http://m.share.zdbjq.cn/Article/details/gzisgyopk.sHtML

[R58] 下载文件
来源：http://www.share.hesvh.cn/Article/details/gicpafawk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fehbvm.com/Article/details/grqwiliwo.sHtML

[R59] 发 POST JSON
来源：http://mobile.hesvh.cn/Article/details/gzkjkxemr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fehbvm.com/Article/details/gthjdrxei.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/gmzjdjonk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.zdbjq.cn/Article/details/gwolfiqtt.sHtML

[R61] 磁盘占用
来源：http://read.share.zdbjq.cn/Article/details/gnxigsqnt.sHtML

df -h;  du -sh *
来源：http://www.blog.hesvh.cn/Article/details/gpeurjvgf.sHtML

[R62] 找最占空间的文件
来源：http://www.share.zdbjq.cn/Article/details/gstpqzhcf.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fehbvm.com/Article/details/gmpaiujbu.sHtML

[R63] 内存与进程
来源：http://3g.fehbvm.com/Article/details/gwowbvujl.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.zdbjq.cn/Article/details/gsedpvcyt.sHtML

[R64] 结束进程
来源：http://read.share.fehbvm.com/Article/details/giyscsleq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.hesvh.cn/Article/details/gtffeswid.sHtML

[R65] 查看端口占用
来源：http://wap.fehbvm.com/Article/details/gwsxiovxp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fehbvm.com/Article/details/gffcfdfhk.sHtML

[R66] 定时任务
来源：http://read.share.zdbjq.cn/Article/details/grfvxmufb.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fehbvm.com/Article/details/gvvyesidu.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fehbvm.com/Article/details/gkzoyorrt.sHtML

openssl rand -hex 16
来源：http://www.share.hesvh.cn/Article/details/gkhqtrekn.sHtML

[R68] 计算文件校验值
来源：http://blog.zdbjq.cn/Article/details/gmynejnqe.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.zdbjq.cn/Article/details/giodtmvmw.sHtML

[R69] 生成随机密码
来源：http://read.share.fehbvm.com/Article/details/gfcbpdygz.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.zdbjq.cn/Article/details/gmcrgglqd.sHtML

[R70] 时间戳与互转
来源：http://mobile.hesvh.cn/Article/details/gbzvjeftv.sHtML

date +%s;  date -d @1700000000
来源：http://3g.hesvh.cn/Article/details/gtmqgrpdg.sHtML

[R71] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/ghazkybql.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.zdbjq.cn/Article/details/grmjyxpew.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.hesvh.cn/Article/details/gsrsjleum.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gyfsybskr.sHtML

[R73] 分割大日志
来源：http://read.share.hesvh.cn/Article/details/govztjelf.sHtML

split -l 1000 big.log part_
来源：http://read.share.hesvh.cn/Article/details/gfinrwweg.sHtML

[R74] 批量重命名
来源：http://www.share.hesvh.cn/Article/details/gidsoperx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.hesvh.cn/Article/details/gtoihdtlu.sHtML

[R75] 导出环境变量
来源：http://read.share.fehbvm.com/Article/details/gltpeqcki.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fehbvm.com/Article/details/gxlrhcqqh.sHtML

[R76] 使用临时文件
来源：http://mobile.zdbjq.cn/Article/details/gycvbyjmi.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.zdbjq.cn/Article/details/gdzeeplvt.sHtML

[R77] 读取用户输入
来源：http://3g.zdbjq.cn/Article/details/grrcuubsh.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.zdbjq.cn/Article/details/gzhxuanxa.sHtML

[R78] 交互式菜单
来源：http://baike.hesvh.cn/Article/details/ghagctlyv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.hesvh.cn/Article/details/gnyoakmcg.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.hesvh.cn/Article/details/gsqidwwap.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fehbvm.com/Article/details/gqpxnyfri.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.zdbjq.cn/Article/details/gjnkbnzda.sHtML

time ./run.sh
来源：http://blog.fehbvm.com/Article/details/ggompwnlh.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gtwwmbpzr.sHtML

S. C / C++ 专题
来源：http://www.share.hesvh.cn/Article/details/gppqyxtyc.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gwpluljdw.sHtML

[S01] C：Hello World
来源：http://wap.hesvh.cn/Article/details/ghllfjgmr.sHtML

#include <stdio.h>
来源：http://www.share.zdbjq.cn/Article/details/gtpscoqmm.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.zdbjq.cn/Article/details/gbvyrktzr.sHtML

[S02] C：变量与格式化输出
来源：http://3g.hesvh.cn/Article/details/grsagqdai.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fehbvm.com/Article/details/gqyyquuam.sHtML

[S03] C：读入整数
来源：http://www.blog.zdbjq.cn/Article/details/guihrajhy.sHtML

int x; scanf("%d", &x);
来源：http://mobile.zdbjq.cn/Article/details/gosjltwnv.sHtML

[S04] C：字符串复制
来源：http://blog.hesvh.cn/Article/details/gyvfafcjr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gqmacnnfp.sHtML

[S05] C：字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/gssdqfnpr.sHtML

strlen(s)
来源：http://www.blog.hesvh.cn/Article/details/gcenucxhw.sHtML

[S06] C：字符串比较
来源：http://www.share.fehbvm.com/Article/details/gyjtwkpvg.sHtML

strcmp(a, b) == 0
来源：http://baike.zdbjq.cn/Article/details/gdrisavms.sHtML

[S07] C：数组遍历求和
来源：http://wap.zdbjq.cn/Article/details/gyvnaxefu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.zdbjq.cn/Article/details/gyeurwxsa.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.hesvh.cn/Article/details/gdyddypzu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.zdbjq.cn/Article/details/gjuetfpes.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.zdbjq.cn/Article/details/gczszscmy.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.zdbjq.cn/Article/details/gzygluxcc.sHtML

[S10] C：指针与解引用
来源：http://mobile.zdbjq.cn/Article/details/gczibeiqh.sHtML

int *p = &a;  *p = 5;
来源：http://blog.hesvh.cn/Article/details/gumfeqytc.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gleqmwyek.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.hesvh.cn/Article/details/ggclwqptd.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.hesvh.cn/Article/details/glivfdehv.sHtML

fclose(f);
来源：http://3g.hesvh.cn/Article/details/ggjhghcwr.sHtML

[S12] C：写文件
来源：http://3g.zdbjq.cn/Article/details/gnpxrjqnh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.zdbjq.cn/Article/details/gdkhquyyf.sHtML

[S13] C：宏定义
来源：http://m.share.hesvh.cn/Article/details/glrfclbzl.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.hesvh.cn/Article/details/gnsbryrgb.sHtML

[S14] C：枚举
来源：http://blog.zdbjq.cn/Article/details/gtvztgemt.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.hesvh.cn/Article/details/geojyjlut.sHtML

[S15] C：类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/garsluhpj.sHtML

(double) a / b
来源：http://mobile.fehbvm.com/Article/details/ghiogzlfw.sHtML

[S16] C：位操作置位
来源：http://m.share.hesvh.cn/Article/details/gdcgdbekn.sHtML

x |= (1 << 3);
来源：http://m.share.zdbjq.cn/Article/details/gbhvutxyf.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gtblqxrll.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.zdbjq.cn/Article/details/ghkouwcpv.sHtML

[S18] C：命令行参数
来源：http://baike.hesvh.cn/Article/details/gkpcmxphg.sHtML

int main(int argc, char **argv)
来源：http://3g.zdbjq.cn/Article/details/govhsvkyg.sHtML

[S19] C：快速排序
来源：http://blog.zdbjq.cn/Article/details/gsmdxxaky.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gtoqbizwp.sHtML

[S20] C：二分查找
来源：http://mobile.hesvh.cn/Article/details/ghrttrvuo.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/gzqawtlem.sHtML

[S21] C：字符类别判断
来源：http://blog.zdbjq.cn/Article/details/gckfptztl.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.hesvh.cn/Article/details/gjwiegbjv.sHtML

[S22] C：字符串转数字
来源：http://www.blog.zdbjq.cn/Article/details/gfyeifjob.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.zdbjq.cn/Article/details/gwkjbcqvz.sHtML

[S23] C：随机数
来源：http://blog.zdbjq.cn/Article/details/giqgcvvjn.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.hesvh.cn/Article/details/gnckhktxh.sHtML

[S24] C：获取本地时间
来源：http://mobile.hesvh.cn/Article/details/gugyyaktj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.hesvh.cn/Article/details/gczycjkls.sHtML

[S25] C：内存拷贝
来源：http://www.share.zdbjq.cn/Article/details/gtjkwsani.sHtML

memcpy(dst, src, n);
来源：http://blog.zdbjq.cn/Article/details/gijehfrqh.sHtML

[S26] C：内存清零
来源：http://www.blog.fehbvm.com/Article/details/glbjovsbs.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fehbvm.com/Article/details/gtnjedsgs.sHtML

[S27] C：定义常量
来源：http://wap.fehbvm.com/Article/details/grgjjpyxd.sHtML

const double PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gitkmpolo.sHtML

[S28] C：静态变量
来源：http://www.m.share.hesvh.cn/Article/details/gbjbqvhbl.sHtML

static int counter = 0;
来源：http://read.share.fehbvm.com/Article/details/gobzylxmz.sHtML

[S29] C：变参函数
来源：http://www.blog.fehbvm.com/Article/details/gespnpxpc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.hesvh.cn/Article/details/gsxsmgslx.sHtML

[S30] C：头文件保护
来源：http://www.blog.fehbvm.com/Article/details/gldfrdtan.sHtML

#ifndef X_H
来源：http://www.blog.fehbvm.com/Article/details/gmcgwbonm.sHtML

#define X_H
来源：http://m.share.hesvh.cn/Article/details/gupmfembc.sHtML

#endif
来源：http://baike.zdbjq.cn/Article/details/gumcunnqm.sHtML

[S31] C++：Hello World
来源：http://mobile.fehbvm.com/Article/details/guvkdmkrz.sHtML

#include <iostream>
来源：http://m.share.fehbvm.com/Article/details/gucbwmgyl.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fehbvm.com/Article/details/gwwovoqtd.sHtML

[S32] C++：字符串
来源：http://read.share.fehbvm.com/Article/details/gadmhhxnd.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.hesvh.cn/Article/details/gxnedudjf.sHtML

[S33] C++：vector 增删
来源：http://wap.hesvh.cn/Article/details/gthrqcffg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.zdbjq.cn/Article/details/gqdjjqnif.sHtML

[S34] C++：遍历 vector
来源：http://wap.zdbjq.cn/Article/details/ghmfqjano.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.zdbjq.cn/Article/details/gstscldxs.sHtML

[S35] C++：map
来源：http://blog.zdbjq.cn/Article/details/gijqawymf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gncbqynab.sHtML

[S36] C++：unordered_map
来源：http://read.share.zdbjq.cn/Article/details/gkthgvlpc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gjugfvsrx.sHtML

[S37] C++：set
来源：http://m.share.zdbjq.cn/Article/details/gvassfzah.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gsmgnjstc.sHtML

[S38] C++：排序
来源：http://www.m.share.zdbjq.cn/Article/details/gnsxyammv.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.zdbjq.cn/Article/details/gnkzzrafd.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fehbvm.com/Article/details/gaikvgzsj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.zdbjq.cn/Article/details/ghlbexvll.sHtML

[S40] C++：查找元素
来源：http://www.blog.zdbjq.cn/Article/details/glgckpcvx.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fehbvm.com/Article/details/gwyclfsdu.sHtML

[S41] C++：类与构造函数
来源：http://m.share.hesvh.cn/Article/details/gzauqixcs.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.zdbjq.cn/Article/details/guckjsimp.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.zdbjq.cn/Article/details/gqsgmawsp.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fehbvm.com/Article/details/gcqkbcvwm.sHtML

[S43] C++：智能指针
来源：http://blog.zdbjq.cn/Article/details/gzenqavvb.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.hesvh.cn/Article/details/geghlmmfb.sHtML

[S44] C++：引用传参
来源：http://blog.zdbjq.cn/Article/details/gosqctffi.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.hesvh.cn/Article/details/gpyaxyoee.sHtML

[S45] C++：lambda
来源：http://3g.zdbjq.cn/Article/details/gsoxhgxbc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.hesvh.cn/Article/details/gsrskfjyz.sHtML

[S46] C++：函数模板
来源：http://www.m.share.zdbjq.cn/Article/details/glshscivf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fehbvm.com/Article/details/gdubjjzqi.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.zdbjq.cn/Article/details/grwuurjgi.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fehbvm.com/Article/details/gisvvmfks.sHtML

[S48] C++：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gfvgzghpp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.hesvh.cn/Article/details/gzttycdcg.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.hesvh.cn/Article/details/gcyxztqfs.sHtML

[S49] C++：写文件
来源：http://wap.hesvh.cn/Article/details/giezconai.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.zdbjq.cn/Article/details/gjhtdqoit.sHtML

[S50] C++：格式化数字
来源：http://3g.hesvh.cn/Article/details/ghvcgpmed.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.hesvh.cn/Article/details/guafhovlw.sHtML

[S51] C++：显式类型转换
来源：http://3g.fehbvm.com/Article/details/gmwexwzht.sHtML

static_cast<double>(a) / b
来源：http://www.share.hesvh.cn/Article/details/gekkfzlmw.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.hesvh.cn/Article/details/gglbzdbot.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fehbvm.com/Article/details/gtfyiudcx.sHtML

[S53] C++：移动语义
来源：http://wap.zdbjq.cn/Article/details/gnkwsghpv.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fehbvm.com/Article/details/ggqefxsqg.sHtML

[S54] C++：异常处理
来源：http://3g.fehbvm.com/Article/details/gkndelozm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.zdbjq.cn/Article/details/gznuzjoow.sHtML

[S55] C++：结构化绑定
来源：http://mobile.zdbjq.cn/Article/details/gddvhuwvd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.zdbjq.cn/Article/details/gbfkzpmjj.sHtML

[S56] C++：optional
来源：http://mobile.fehbvm.com/Article/details/gzrafbxpt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fehbvm.com/Article/details/gcmwnunlh.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.hesvh.cn/Article/details/gaipebtua.sHtML

constexpr int N = 10;
来源：http://blog.zdbjq.cn/Article/details/gkxesnvvb.sHtML

[S58] C++：命名空间
来源：http://www.blog.zdbjq.cn/Article/details/grtqmjchu.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fehbvm.com/Article/details/gvmiiqljr.sHtML

[S59] C++：静态断言
来源：http://www.share.hesvh.cn/Article/details/gthmmuycp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.zdbjq.cn/Article/details/ggskosfrz.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.zdbjq.cn/Article/details/gcmbpgxjx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.zdbjq.cn/Article/details/gjmogvomn.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gevgtsulv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/gyxsaoupe.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gzuetkmcf.sHtML

[T01] Kotlin：Hello World
来源：http://3g.zdbjq.cn/Article/details/gcpimgniv.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/glqlezzma.sHtML

[T02] Kotlin：变量
来源：http://www.share.zdbjq.cn/Article/details/gpgrijxzz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fehbvm.com/Article/details/gghlmowba.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fehbvm.com/Article/details/grwozmpmx.sHtML

"值: $b"
来源：http://read.share.hesvh.cn/Article/details/goozodvcm.sHtML

[T04] Kotlin：空安全
来源：http://3g.fehbvm.com/Article/details/gidxswzzq.sHtML

val n: String? = null;  n?.length
来源：http://baike.fehbvm.com/Article/details/gpiuglesu.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.hesvh.cn/Article/details/gytfquxgd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.hesvh.cn/Article/details/gybdukiwz.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.hesvh.cn/Article/details/goswnihae.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fehbvm.com/Article/details/ghvtunlhg.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.zdbjq.cn/Article/details/gpnputtuu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.hesvh.cn/Article/details/gwnjgxqdq.sHtML

[T08] Kotlin：数据类
来源：http://baike.zdbjq.cn/Article/details/gmhthiyli.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.zdbjq.cn/Article/details/gihiwsuzw.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.zdbjq.cn/Article/details/glunyrggh.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fehbvm.com/Article/details/gkwohqqwl.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fehbvm.com/Article/details/gekyxywrn.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fehbvm.com/Article/details/ghiybwynj.sHtML

[T11] Kotlin：协程
来源：http://blog.hesvh.cn/Article/details/gyebjyycn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fehbvm.com/Article/details/gpohhhocd.sHtML

[T12] Kotlin：解构声明
来源：http://wap.hesvh.cn/Article/details/gokjyljfy.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gzkcvcejn.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.zdbjq.cn/Article/details/gtpuvqqgz.sHtML

val m = mapOf("a" to 1)
来源：http://3g.zdbjq.cn/Article/details/gieqnfpvn.sHtML

[T14] Kotlin：循环
来源：http://3g.fehbvm.com/Article/details/gvzhfuxes.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fehbvm.com/Article/details/gmetyyqgg.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fehbvm.com/Article/details/gadogqurr.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fehbvm.com/Article/details/gmmlnvlry.sHtML

[T16] Swift：Hello World
来源：http://www.share.fehbvm.com/Article/details/gqwcpdpih.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gyeamhjap.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fehbvm.com/Article/details/gyqfcryao.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fehbvm.com/Article/details/grhzagarh.sHtML

[T18] Swift：字符串插值
来源：http://wap.fehbvm.com/Article/details/gqxravjwl.sHtML

"值: \(b)"
来源：http://read.share.zdbjq.cn/Article/details/gigoepcmv.sHtML

[T19] Swift：可选绑定
来源：http://m.share.hesvh.cn/Article/details/ghdhfpaum.sHtML

if let n = opt { print(n) }
来源：http://www.share.fehbvm.com/Article/details/gdihmwwus.sHtML

[T20] Swift：数组操作
来源：http://m.share.fehbvm.com/Article/details/gzqrbarpz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fehbvm.com/Article/details/gcnxbhjdg.sHtML

[T21] Swift：遍历
来源：http://mobile.hesvh.cn/Article/details/giivgxegu.sHtML

for x in a { print(x) }
来源：http://www.share.fehbvm.com/Article/details/guuwbcpou.sHtML

[T22] Swift：字典
来源：http://blog.hesvh.cn/Article/details/gwlmztzyy.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fehbvm.com/Article/details/gshtvoxpy.sHtML

[T23] Swift：函数
来源：http://mobile.zdbjq.cn/Article/details/gdcmadmfb.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.hesvh.cn/Article/details/gtkmcblzi.sHtML

[T24] Swift：闭包
来源：http://3g.zdbjq.cn/Article/details/goyhrzvag.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.hesvh.cn/Article/details/gezgktaud.sHtML

[T25] Swift：结构体
来源：http://3g.hesvh.cn/Article/details/gplcumkln.sHtML

struct P { var x: Int }
来源：http://www.share.hesvh.cn/Article/details/gpnxnsmus.sHtML

[T26] Swift：类与重写
来源：http://m.share.fehbvm.com/Article/details/gnettezzf.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.zdbjq.cn/Article/details/gsqlbzvmk.sHtML

[T27] Swift：错误处理
来源：http://www.blog.hesvh.cn/Article/details/gyulwncaj.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fehbvm.com/Article/details/grouhrxai.sHtML

[T28] Swift：枚举
来源：http://www.share.zdbjq.cn/Article/details/gruahvvxr.sHtML

enum Color { case red, green }
来源：http://wap.hesvh.cn/Article/details/gnpdwioim.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fehbvm.com/Article/details/gkmzarihf.sHtML

guard let x = opt else { return }
来源：http://blog.hesvh.cn/Article/details/gqchvxtli.sHtML

[T30] Swift：协议
来源：http://www.m.share.fehbvm.com/Article/details/gmanrtwct.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fehbvm.com/Article/details/geyyorhok.sHtML

[T31] Lua：Hello World
来源：http://blog.hesvh.cn/Article/details/gttiaupki.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/goesrkyyb.sHtML

[T32] Lua：局部变量
来源：http://m.share.fehbvm.com/Article/details/gxqkzzmud.sHtML

local a = 1
来源：http://www.m.share.zdbjq.cn/Article/details/glenpiefu.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.hesvh.cn/Article/details/gsgufkrxs.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fehbvm.com/Article/details/gokwfaqoo.sHtML

[T34] Lua：遍历表
来源：http://baike.hesvh.cn/Article/details/geotpegea.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.hesvh.cn/Article/details/gsbnizfkf.sHtML


<!-- 参考信息 -->