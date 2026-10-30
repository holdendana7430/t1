代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fanxiaobao.xyz/Article/details/goifjgcdd.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/glrujavhl.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fanxiaobao.xyz/Article/details/gxuozlokd.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gftbzyuhu.sHtML

files=$(ls -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbthamqqu.sHtML

[R38] 管道串联
来源：http://mobile.fanxiaobao.xyz/Article/details/ggyjetdkf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjixrqbbj.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqvvqagpz.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpnnknbto.sHtML

[R40] 追加写日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahadyfue.sHtML

echo "log" >> out.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gbgqofhcj.sHtML

[R41] 丢弃输出
来源：http://blog.fanxiaobao.xyz/Article/details/gwwcrfsxa.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/grqrdhjbn.sHtML

[R42] 输入重定向
来源：http://www.blog.fanxiaobao.xyz/Article/details/gknzynsot.sHtML

wc -l < a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gpdnwnlva.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/giexwczwx.sHtML

find . -name "*.log" -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/ghsogrthw.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpitiwdce.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gbcncgocl.sHtML

[R45] 批量删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gluesnzri.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fanxiaobao.xyz/Article/details/gypttuqqh.sHtML

[R46] 递归替换文件内容
来源：http://blog.fanxiaobao.xyz/Article/details/gegqnbspv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/guhirplrv.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gqfzthpgk.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gppefztdk.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gpxofudct.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/guyiqliih.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gylbtwpyo.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fanxiaobao.xyz/Article/details/gqokluxsa.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvqeupnv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gbffrznla.sHtML

[R51] 排序去重取前几
来源：http://wap.fanxiaobao.xyz/Article/details/gktupfouz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gszxaecrk.sHtML

[R52] 统计行数
来源：http://read.share.fanxiaobao.xyz/Article/details/gkltvetxn.sHtML

wc -l a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gyihdvsub.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fanxiaobao.xyz/Article/details/gcfczzoqr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gwynulcco.sHtML

[R54] 比较两个文件
来源：http://blog.fanxiaobao.xyz/Article/details/glikvofjj.sHtML

diff a.txt b.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glkrgxgiq.sHtML

[R55] 压缩与解压
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvglrhupv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxclxwanw.sHtML

[R56] 远程拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxumohned.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/gokoixsnh.sHtML

[R57] 远程执行命令
来源：http://baike.fanxiaobao.xyz/Article/details/gzuwhffss.sHtML

ssh user@host 'uptime'
来源：http://www.share.fanxiaobao.xyz/Article/details/gnurepdtz.sHtML

[R58] 下载文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkxyfjpvo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fanxiaobao.xyz/Article/details/gmrntqird.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gitkpjzag.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/geiclgvpj.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxkdkhnhz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fanxiaobao.xyz/Article/details/gpmryxkvz.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkukuuxef.sHtML

df -h;  du -sh *
来源：http://m.share.fanxiaobao.xyz/Article/details/guaylophg.sHtML

[R62] 找最占空间的文件
来源：http://blog.fanxiaobao.xyz/Article/details/gwlmebhik.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fanxiaobao.xyz/Article/details/goulgctgz.sHtML

[R63] 内存与进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gnalltrks.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fanxiaobao.xyz/Article/details/gfmoyvpsy.sHtML

[R64] 结束进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gpsxsecif.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fanxiaobao.xyz/Article/details/ggrewevve.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gttvqznet.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fanxiaobao.xyz/Article/details/gndnrmkii.sHtML

[R66] 定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/gppuaqfyk.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnagmhjpm.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fanxiaobao.xyz/Article/details/gorszfvoa.sHtML

openssl rand -hex 16
来源：http://mobile.fanxiaobao.xyz/Article/details/gbnummjtg.sHtML

[R68] 计算文件校验值
来源：http://m.share.fanxiaobao.xyz/Article/details/gmtgcpfkx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gsksxteqy.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glcxubyce.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gombywpfe.sHtML

[R70] 时间戳与互转
来源：http://wap.fanxiaobao.xyz/Article/details/gvvvxgkpc.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzgftezxk.sHtML

[R71] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdpqiatvo.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fanxiaobao.xyz/Article/details/gzpuxsjtm.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/gpigpeqfq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmgdanlvj.sHtML

[R73] 分割大日志
来源：http://wap.fanxiaobao.xyz/Article/details/gyutusmlk.sHtML

split -l 1000 big.log part_
来源：http://3g.fanxiaobao.xyz/Article/details/gbfroxuqy.sHtML

[R74] 批量重命名
来源：http://read.share.fanxiaobao.xyz/Article/details/gyhlmzdml.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gbrkoljyw.sHtML

[R75] 导出环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gjfpnxgmr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fanxiaobao.xyz/Article/details/grlmbilrs.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfbcmdcql.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gtaeaibra.sHtML

[R77] 读取用户输入
来源：http://read.share.fanxiaobao.xyz/Article/details/gnhoxyuzy.sHtML

read -rp "请输入: " ans
来源：http://baike.fanxiaobao.xyz/Article/details/gsmdpwcqu.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqvisvxlh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghoyiihge.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fanxiaobao.xyz/Article/details/gijufopki.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fanxiaobao.xyz/Article/details/ghkeqxiyw.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fanxiaobao.xyz/Article/details/ggftexamx.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/gltxkvhqb.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gunfdcvyq.sHtML

S. C / C++ 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gmxctyjzf.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/glpwxxpeu.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gqpxsbfrr.sHtML

#include <stdio.h>
来源：http://mobile.fanxiaobao.xyz/Article/details/gvvdkngep.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grvcwaxwg.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhejcsqe.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fanxiaobao.xyz/Article/details/gsstrtkot.sHtML

[S03] C：读入整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvhpkqtsz.sHtML

int x; scanf("%d", &x);
来源：http://baike.fanxiaobao.xyz/Article/details/gnqmjghzu.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbcauocho.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzpembpyy.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/getbvhhgv.sHtML

strlen(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gsuxenwcr.sHtML

[S06] C：字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdllxdnjq.sHtML

strcmp(a, b) == 0
来源：http://baike.fanxiaobao.xyz/Article/details/glytpbzdh.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gcpurjufa.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fanxiaobao.xyz/Article/details/gebxnkagf.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fanxiaobao.xyz/Article/details/gpogvmoak.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcydyguke.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fanxiaobao.xyz/Article/details/gahdzyawk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcmgbyfyx.sHtML

[S10] C：指针与解引用
来源：http://m.share.fanxiaobao.xyz/Article/details/gbguyhsln.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gugyarzgi.sHtML

[S11] C：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/giqvwpafl.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/gzvqinvyp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gftoaewas.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnzxsnrcv.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gkkhycnbv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gkfuqvezh.sHtML

[S13] C：宏定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gtvemgazd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fanxiaobao.xyz/Article/details/gvslcconi.sHtML

[S14] C：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnprssycm.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fanxiaobao.xyz/Article/details/gnyaqkxkv.sHtML

[S15] C：类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gbunwpnhu.sHtML

(double) a / b
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtkbsrpu.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbdsdkunt.sHtML

x |= (1 << 3);
来源：http://blog.fanxiaobao.xyz/Article/details/ghqyoeskj.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/guuoogrrh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fanxiaobao.xyz/Article/details/gujwjpcgt.sHtML

[S18] C：命令行参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gxoltawpa.sHtML

int main(int argc, char **argv)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzugalnrv.sHtML

[S19] C：快速排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gbyrnhyjo.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gebkwunsw.sHtML

[S20] C：二分查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gwyqgsdde.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvclbylm.sHtML

[S21] C：字符类别判断
来源：http://baike.fanxiaobao.xyz/Article/details/glflqwirw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fanxiaobao.xyz/Article/details/grofikicl.sHtML

[S22] C：字符串转数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gebewglmq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fanxiaobao.xyz/Article/details/gwzaimdho.sHtML

[S23] C：随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gecfxwnjc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gtfjxdmyg.sHtML

[S24] C：获取本地时间
来源：http://mobile.fanxiaobao.xyz/Article/details/goiwoibbi.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fanxiaobao.xyz/Article/details/gyzdnhokn.sHtML

[S25] C：内存拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gcffmgqlh.sHtML

memcpy(dst, src, n);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzyuktymq.sHtML

[S26] C：内存清零
来源：http://m.share.fanxiaobao.xyz/Article/details/guvefzail.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fanxiaobao.xyz/Article/details/guqhemnlt.sHtML

[S27] C：定义常量
来源：http://baike.fanxiaobao.xyz/Article/details/gvmypzlkq.sHtML

const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ginrsxewe.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/gqtogypax.sHtML

static int counter = 0;
来源：http://baike.fanxiaobao.xyz/Article/details/gfkftilmc.sHtML

[S29] C：变参函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyeqsfqqd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fanxiaobao.xyz/Article/details/giahjylel.sHtML

[S30] C：头文件保护
来源：http://mobile.fanxiaobao.xyz/Article/details/getpghmkg.sHtML

#ifndef X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gwuekvuxr.sHtML

#define X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gbfebfyyv.sHtML

#endif
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpfzgkccd.sHtML

[S31] C++：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gyykqrwrn.sHtML

#include <iostream>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gobumyciu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggnbufrli.sHtML

[S32] C++：字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gavcvhnbl.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fanxiaobao.xyz/Article/details/gqoxrngzc.sHtML

[S33] C++：vector 增删
来源：http://www.share.fanxiaobao.xyz/Article/details/gclvdytkq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gubpjngtv.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fanxiaobao.xyz/Article/details/gekwxepfm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gfmsjbxdg.sHtML

[S35] C++：map
来源：http://blog.fanxiaobao.xyz/Article/details/gfxcpntui.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gutmodpem.sHtML

[S36] C++：unordered_map
来源：http://wap.fanxiaobao.xyz/Article/details/grsdslzid.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcnssbogc.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/gtemifbhl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fanxiaobao.xyz/Article/details/groxzujno.sHtML

[S38] C++：排序
来源：http://baike.fanxiaobao.xyz/Article/details/gvrgqntpn.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gunjkwtnc.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gfgercdhz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fanxiaobao.xyz/Article/details/gzckzamzp.sHtML

[S40] C++：查找元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gafcmufrn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gihklllxk.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbqftitu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fanxiaobao.xyz/Article/details/gxbdtouhg.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fanxiaobao.xyz/Article/details/grbfdwiyg.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/gmcxzlsiv.sHtML

[S43] C++：智能指针
来源：http://3g.fanxiaobao.xyz/Article/details/gekmkanxf.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fanxiaobao.xyz/Article/details/guuqcxvnz.sHtML

[S44] C++：引用传参
来源：http://wap.fanxiaobao.xyz/Article/details/gwvtlhrsf.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdoqvecvc.sHtML

[S45] C++：lambda
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpkxlqqtu.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fanxiaobao.xyz/Article/details/gupabvbpf.sHtML

[S46] C++：函数模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gwcahniuw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjaxykgc.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gddcenxce.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbaorooux.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/guxasitqf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fanxiaobao.xyz/Article/details/gtzazllgh.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbvhgkgkd.sHtML

[S49] C++：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gzvpiajiz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gwnnsxxhe.sHtML

[S50] C++：格式化数字
来源：http://3g.fanxiaobao.xyz/Article/details/gmrhlxnhy.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwpgrfxg.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbyfrccjx.sHtML

static_cast<double>(a) / b
来源：http://blog.fanxiaobao.xyz/Article/details/gdnqewkjo.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fanxiaobao.xyz/Article/details/ginksuzwl.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fanxiaobao.xyz/Article/details/gfwrtymff.sHtML

[S53] C++：移动语义
来源：http://wap.fanxiaobao.xyz/Article/details/gjwtbuzwl.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fanxiaobao.xyz/Article/details/ggxsqpatg.sHtML

[S54] C++：异常处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwgbloxf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gywquhkct.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpnlwhgnq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gnlpbbkco.sHtML

[S56] C++：optional
来源：http://www.share.fanxiaobao.xyz/Article/details/gqdncnuxy.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gubhzxmpb.sHtML

[S57] C++：编译期常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gmoapmmop.sHtML

constexpr int N = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gursztvoh.sHtML

[S58] C++：命名空间
来源：http://3g.fanxiaobao.xyz/Article/details/gsnukfblo.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fanxiaobao.xyz/Article/details/gnmdmbqcd.sHtML

[S59] C++：静态断言
来源：http://baike.fanxiaobao.xyz/Article/details/gwsultlxd.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fanxiaobao.xyz/Article/details/gsngflkli.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fanxiaobao.xyz/Article/details/ghqlyzgph.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gpxpvbfgy.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gymbgheko.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvdapoxqp.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/goumjipjh.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gfarxnpyq.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsgwhajia.sHtML

[T02] Kotlin：变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gxdqgogcm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghfuysyrk.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fanxiaobao.xyz/Article/details/guzevqdhh.sHtML

"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gllkaorqm.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fanxiaobao.xyz/Article/details/gwrnzglun.sHtML

val n: String? = null;  n?.length
来源：http://wap.fanxiaobao.xyz/Article/details/gfmukzojy.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gltsawgwr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fanxiaobao.xyz/Article/details/glozzbofl.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/guylecfuu.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gieedqhqb.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gckkowxuw.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fanxiaobao.xyz/Article/details/gchrpuyfc.sHtML

[T08] Kotlin：数据类
来源：http://blog.fanxiaobao.xyz/Article/details/giikfxppi.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/gzrhhiusc.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gbhzfhkao.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fanxiaobao.xyz/Article/details/glvawfaop.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fanxiaobao.xyz/Article/details/gqcqdgvat.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gevuwctjr.sHtML

[T11] Kotlin：协程
来源：http://baike.fanxiaobao.xyz/Article/details/gqgfqfizc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fanxiaobao.xyz/Article/details/gxqajemkh.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fanxiaobao.xyz/Article/details/guizepqoh.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gqqzahqxb.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fanxiaobao.xyz/Article/details/gwlqpobxb.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gxxfgjjyi.sHtML

[T14] Kotlin：循环
来源：http://baike.fanxiaobao.xyz/Article/details/gyiyqmpif.sHtML

for (i in 1..10) println(i)
来源：http://wap.fanxiaobao.xyz/Article/details/glbqzagez.sHtML

[T15] Kotlin：接口
来源：http://baike.fanxiaobao.xyz/Article/details/gqlcwmvhz.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fanxiaobao.xyz/Article/details/gwbjcjglr.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdfkizrlr.sHtML

print("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfflhyxyl.sHtML

[T17] Swift：变量与常量
来源：http://3g.fanxiaobao.xyz/Article/details/geuzsqihq.sHtML

var a = 1;  let b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/glazgvcqe.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gaikwnsjw.sHtML

"值: \(b)"
来源：http://wap.fanxiaobao.xyz/Article/details/goizcngjm.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggtduooki.sHtML

if let n = opt { print(n) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gldtrzecs.sHtML

[T20] Swift：数组操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gstzocntr.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwnpwden.sHtML

[T21] Swift：遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnajsltt.sHtML

for x in a { print(x) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgvblrzg.sHtML

[T22] Swift：字典
来源：http://blog.fanxiaobao.xyz/Article/details/gmrhijkiv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gfodnstmm.sHtML

[T23] Swift：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gzwvsnosz.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtbdciytc.sHtML

[T24] Swift：闭包
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmytwkqqz.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/gjjckfrbo.sHtML

[T25] Swift：结构体
来源：http://www.blog.fanxiaobao.xyz/Article/details/gviizvlma.sHtML

struct P { var x: Int }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtmcfljjy.sHtML

[T26] Swift：类与重写
来源：http://3g.fanxiaobao.xyz/Article/details/gijeafgdb.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsxwbaxgu.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/girrnqfli.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fanxiaobao.xyz/Article/details/guknenajm.sHtML

[T28] Swift：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gmkyccttx.sHtML

enum Color { case red, green }
来源：http://wap.fanxiaobao.xyz/Article/details/gpqpkbmog.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fanxiaobao.xyz/Article/details/guiwlugkj.sHtML

guard let x = opt else { return }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwhavlqk.sHtML

[T30] Swift：协议
来源：http://3g.fanxiaobao.xyz/Article/details/gktzaszdu.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fanxiaobao.xyz/Article/details/gdsykhijr.sHtML

[T31] Lua：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gkrlkejzm.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/grpvmamzr.sHtML

[T32] Lua：局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gfveabmgy.sHtML

local a = 1
来源：http://blog.fanxiaobao.xyz/Article/details/gtahddnaz.sHtML

[T33] Lua：表（数组）
来源：http://baike.fanxiaobao.xyz/Article/details/ghrkyffcv.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fanxiaobao.xyz/Article/details/gfhhjbxqx.sHtML

[T34] Lua：遍历表
来源：http://3g.fanxiaobao.xyz/Article/details/gnryojumf.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fanxiaobao.xyz/Article/details/gzycvswwq.sHtML

[T35] Lua：字典表
来源：http://wap.fanxiaobao.xyz/Article/details/gcnnrnlxr.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gqewszrte.sHtML

[T36] Lua：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsukvxgop.sHtML

function add(a, b) return a + b end
来源：http://mobile.fanxiaobao.xyz/Article/details/gqihbswln.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/gbhzthsgz.sHtML

"a" .. "b"
来源：http://read.share.fanxiaobao.xyz/Article/details/ggawoqinh.sHtML

[T38] Lua：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjgzxysu.sHtML

if x > 0 then print("正") end
来源：http://blog.fanxiaobao.xyz/Article/details/gdedyqxgp.sHtML


<!-- 参考信息 -->