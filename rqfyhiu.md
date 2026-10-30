代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fehbvm.com/Article/details/grukallfb.sHtML

[R34] 退出时清理
来源：http://wap.zdbjq.cn/Article/details/gcwemwyqt.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/guyuvumyl.sHtML

[R35] 后台执行并等待
来源：http://www.blog.hesvh.cn/Article/details/gxfmwkljj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fehbvm.com/Article/details/gdnphpfwu.sHtML

[R36] 并发执行多个任务
来源：http://blog.zdbjq.cn/Article/details/gxpdwipgb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.zdbjq.cn/Article/details/glbqlhpbq.sHtML

[R37] 把输出赋给变量
来源：http://baike.hesvh.cn/Article/details/gqqoncvnt.sHtML

files=$(ls -1)
来源：http://wap.fehbvm.com/Article/details/gudvbkzup.sHtML

[R38] 管道串联
来源：http://www.m.share.fehbvm.com/Article/details/giimqhqsf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.hesvh.cn/Article/details/gkrhwysjb.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.hesvh.cn/Article/details/gnpcafpza.sHtML

cmd > out.log 2>&1
来源：http://wap.fehbvm.com/Article/details/gwkjeblvz.sHtML

[R40] 追加写日志
来源：http://blog.fehbvm.com/Article/details/gtuhtvzzg.sHtML

echo "log" >> out.log
来源：http://3g.zdbjq.cn/Article/details/gwocapywg.sHtML

[R41] 丢弃输出
来源：http://mobile.hesvh.cn/Article/details/gmfditvoe.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/gqnjjbtxf.sHtML

[R42] 输入重定向
来源：http://mobile.zdbjq.cn/Article/details/gvuipbosp.sHtML

wc -l < a.txt
来源：http://3g.hesvh.cn/Article/details/gbdobpvrc.sHtML

[R43] 按名字查找文件
来源：http://blog.fehbvm.com/Article/details/gnejrhssj.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fehbvm.com/Article/details/grfpzrcfj.sHtML

[R44] 按修改时间查找
来源：http://wap.fehbvm.com/Article/details/gnocseeaz.sHtML

find . -mtime -7 -type f
来源：http://m.share.zdbjq.cn/Article/details/gzgfzirfj.sHtML

[R45] 批量删除
来源：http://read.share.hesvh.cn/Article/details/gsdrppuwq.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fehbvm.com/Article/details/gunaeazht.sHtML

[R46] 递归替换文件内容
来源：http://wap.zdbjq.cn/Article/details/ggymgojrv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fehbvm.com/Article/details/gyohwyvdz.sHtML

[R47] sed 单行替换
来源：http://baike.zdbjq.cn/Article/details/gapwjfftd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gyvyyuovc.sHtML

[R48] awk 取指定列
来源：http://read.share.fehbvm.com/Article/details/guymhjgsu.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.hesvh.cn/Article/details/gzlceorwo.sHtML

[R49] awk 带条件
来源：http://www.blog.hesvh.cn/Article/details/gowooxvfx.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.hesvh.cn/Article/details/gbhvdnssd.sHtML

[R50] awk 求和
来源：http://baike.fehbvm.com/Article/details/gyxpddbni.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gohieyvmv.sHtML

[R51] 排序去重取前几
来源：http://3g.fehbvm.com/Article/details/gsmazcsqk.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.zdbjq.cn/Article/details/gtofrhowv.sHtML

[R52] 统计行数
来源：http://www.m.share.hesvh.cn/Article/details/grgvndljx.sHtML

wc -l a.txt
来源：http://mobile.zdbjq.cn/Article/details/geitcuxji.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.hesvh.cn/Article/details/ggjtqaimb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.hesvh.cn/Article/details/gzygzezac.sHtML

[R54] 比较两个文件
来源：http://www.blog.hesvh.cn/Article/details/guydwwshl.sHtML

diff a.txt b.txt
来源：http://www.m.share.hesvh.cn/Article/details/ggpiyaqlq.sHtML

[R55] 压缩与解压
来源：http://blog.hesvh.cn/Article/details/gheejipgr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.zdbjq.cn/Article/details/grqqnpjsr.sHtML

[R56] 远程拷贝
来源：http://read.share.zdbjq.cn/Article/details/ggdwoyili.sHtML

scp file user@host:/path/
来源：http://www.m.share.fehbvm.com/Article/details/gnqdfphau.sHtML

[R57] 远程执行命令
来源：http://www.share.fehbvm.com/Article/details/gexyewvsm.sHtML

ssh user@host 'uptime'
来源：http://baike.hesvh.cn/Article/details/gwbkhwmti.sHtML

[R58] 下载文件
来源：http://read.share.zdbjq.cn/Article/details/gagntggrr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.hesvh.cn/Article/details/gzxaotrpt.sHtML

[R59] 发 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/gppqntvsx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.zdbjq.cn/Article/details/gdfvucrgb.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.hesvh.cn/Article/details/gnimiewea.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.zdbjq.cn/Article/details/gwagoozca.sHtML

[R61] 磁盘占用
来源：http://read.share.fehbvm.com/Article/details/gtvkjpwmn.sHtML

df -h;  du -sh *
来源：http://mobile.zdbjq.cn/Article/details/grkamwgrh.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.zdbjq.cn/Article/details/gcvhzilco.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.hesvh.cn/Article/details/gndvkfuok.sHtML

[R63] 内存与进程
来源：http://www.share.fehbvm.com/Article/details/ggbbghrrp.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fehbvm.com/Article/details/gavpcijlj.sHtML

[R64] 结束进程
来源：http://blog.zdbjq.cn/Article/details/gtgligiqn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.zdbjq.cn/Article/details/gvbokkgdl.sHtML

[R65] 查看端口占用
来源：http://mobile.hesvh.cn/Article/details/gbmddatnq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.hesvh.cn/Article/details/gbzlaukil.sHtML

[R66] 定时任务
来源：http://read.share.hesvh.cn/Article/details/gogbjxclo.sHtML

crontab -e;  crontab -l
来源：http://wap.fehbvm.com/Article/details/gqetlmvfa.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fehbvm.com/Article/details/galiqzwqs.sHtML

openssl rand -hex 16
来源：http://baike.fehbvm.com/Article/details/ggsxgphqy.sHtML

[R68] 计算文件校验值
来源：http://read.share.zdbjq.cn/Article/details/ghdjhkpeu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.zdbjq.cn/Article/details/geyvriepd.sHtML

[R69] 生成随机密码
来源：http://mobile.fehbvm.com/Article/details/grfmbafkc.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fehbvm.com/Article/details/gmwhpczpz.sHtML

[R70] 时间戳与互转
来源：http://read.share.fehbvm.com/Article/details/gifdwskat.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.hesvh.cn/Article/details/gkpufomqd.sHtML

[R71] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gfywggnvf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.zdbjq.cn/Article/details/gqkgyphhr.sHtML

[R72] 等待端口就绪
来源：http://m.share.hesvh.cn/Article/details/gyfubypwn.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/gwwzbbkda.sHtML

[R73] 分割大日志
来源：http://read.share.fehbvm.com/Article/details/gfedlulmd.sHtML

split -l 1000 big.log part_
来源：http://www.share.zdbjq.cn/Article/details/gfycgbbhc.sHtML

[R74] 批量重命名
来源：http://www.share.fehbvm.com/Article/details/gweojmlbv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.hesvh.cn/Article/details/gsuxcgflm.sHtML

[R75] 导出环境变量
来源：http://baike.zdbjq.cn/Article/details/gbcnwoobn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fehbvm.com/Article/details/gyiplrcqi.sHtML

[R76] 使用临时文件
来源：http://blog.zdbjq.cn/Article/details/gbqdxhvba.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gtdozfvfl.sHtML

[R77] 读取用户输入
来源：http://www.share.zdbjq.cn/Article/details/gndpcjefk.sHtML

read -rp "请输入: " ans
来源：http://3g.fehbvm.com/Article/details/grehorwux.sHtML

[R78] 交互式菜单
来源：http://3g.zdbjq.cn/Article/details/grkekrasx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.zdbjq.cn/Article/details/gkfokqvck.sHtML

[R79] 解析命令行选项
来源：http://m.share.zdbjq.cn/Article/details/gndgdoirn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.hesvh.cn/Article/details/gylneicvz.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.zdbjq.cn/Article/details/gjrqdyzid.sHtML

time ./run.sh
来源：http://www.share.zdbjq.cn/Article/details/ggqaksswf.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gceyevmqt.sHtML

S. C / C++ 专题
来源：http://www.share.fehbvm.com/Article/details/grqzqjpww.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ghvgorujr.sHtML

[S01] C：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gfpuznubi.sHtML

#include <stdio.h>
来源：http://www.share.hesvh.cn/Article/details/gooiuqxnw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.hesvh.cn/Article/details/gzhnoltrt.sHtML

[S02] C：变量与格式化输出
来源：http://baike.hesvh.cn/Article/details/gppocbvkq.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.hesvh.cn/Article/details/gpoeciqng.sHtML

[S03] C：读入整数
来源：http://www.blog.fehbvm.com/Article/details/gvskqmvhn.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fehbvm.com/Article/details/gwoxugult.sHtML

[S04] C：字符串复制
来源：http://www.blog.fehbvm.com/Article/details/ggxiqquyj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.hesvh.cn/Article/details/gtkqersvp.sHtML

[S05] C：字符串长度
来源：http://m.share.zdbjq.cn/Article/details/grwwymcom.sHtML

strlen(s)
来源：http://www.m.share.hesvh.cn/Article/details/ghyjrsnhg.sHtML

[S06] C：字符串比较
来源：http://www.share.hesvh.cn/Article/details/ghyzlytqs.sHtML

strcmp(a, b) == 0
来源：http://www.share.zdbjq.cn/Article/details/gmxteviwi.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.zdbjq.cn/Article/details/gnrjviyat.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fehbvm.com/Article/details/gensvixdk.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fehbvm.com/Article/details/gmnvmbtdo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.hesvh.cn/Article/details/gnjhovwhv.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.zdbjq.cn/Article/details/glvaxsnxg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fehbvm.com/Article/details/gzeciopqn.sHtML

[S10] C：指针与解引用
来源：http://wap.fehbvm.com/Article/details/ggzhxprtn.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.zdbjq.cn/Article/details/ghvpcbrub.sHtML

[S11] C：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gnagtkdpd.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fehbvm.com/Article/details/gincbizzk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.hesvh.cn/Article/details/gnnrvgvwx.sHtML

fclose(f);
来源：http://wap.hesvh.cn/Article/details/godorgqoc.sHtML

[S12] C：写文件
来源：http://wap.fehbvm.com/Article/details/ghrmnjrgx.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gojdeyeyq.sHtML

[S13] C：宏定义
来源：http://read.share.zdbjq.cn/Article/details/gbyrwpvmz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.hesvh.cn/Article/details/gijvlmfre.sHtML

[S14] C：枚举
来源：http://m.share.hesvh.cn/Article/details/gdikvccpo.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fehbvm.com/Article/details/glszppyuc.sHtML

[S15] C：类型转换
来源：http://www.m.share.fehbvm.com/Article/details/gxcayugnr.sHtML

(double) a / b
来源：http://m.share.hesvh.cn/Article/details/gzcatgbwy.sHtML

[S16] C：位操作置位
来源：http://blog.zdbjq.cn/Article/details/gikjvppax.sHtML

x |= (1 << 3);
来源：http://mobile.fehbvm.com/Article/details/gkqwqhgzx.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fehbvm.com/Article/details/ggnontbzz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fehbvm.com/Article/details/gqjotqxom.sHtML

[S18] C：命令行参数
来源：http://m.share.fehbvm.com/Article/details/grmithgkt.sHtML

int main(int argc, char **argv)
来源：http://www.share.fehbvm.com/Article/details/gpukzaewi.sHtML

[S19] C：快速排序
来源：http://mobile.zdbjq.cn/Article/details/gvdofvaai.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/gqeonswmz.sHtML

[S20] C：二分查找
来源：http://wap.hesvh.cn/Article/details/gglbfwfew.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/glgwmsgnv.sHtML

[S21] C：字符类别判断
来源：http://baike.hesvh.cn/Article/details/gtcsqsioq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.zdbjq.cn/Article/details/gozrrwqdc.sHtML

[S22] C：字符串转数字
来源：http://baike.zdbjq.cn/Article/details/gpogrzssz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fehbvm.com/Article/details/gvevqvdvd.sHtML

[S23] C：随机数
来源：http://blog.hesvh.cn/Article/details/gpjptbvyd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fehbvm.com/Article/details/gepcxmgkt.sHtML

[S24] C：获取本地时间
来源：http://mobile.fehbvm.com/Article/details/gavzmjxva.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.hesvh.cn/Article/details/gmnxjwziw.sHtML

[S25] C：内存拷贝
来源：http://baike.hesvh.cn/Article/details/gtxrldfsz.sHtML

memcpy(dst, src, n);
来源：http://read.share.hesvh.cn/Article/details/gxedhrwgc.sHtML

[S26] C：内存清零
来源：http://blog.zdbjq.cn/Article/details/gldlrwhye.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.hesvh.cn/Article/details/gunzuvwrm.sHtML

[S27] C：定义常量
来源：http://read.share.hesvh.cn/Article/details/genctzokd.sHtML

const double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gjukpzitz.sHtML

[S28] C：静态变量
来源：http://baike.fehbvm.com/Article/details/gaiahdgtg.sHtML

static int counter = 0;
来源：http://m.share.fehbvm.com/Article/details/gjtwjfeum.sHtML

[S29] C：变参函数
来源：http://www.m.share.hesvh.cn/Article/details/ggpzqnqdq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.zdbjq.cn/Article/details/gznvvfstr.sHtML

[S30] C：头文件保护
来源：http://baike.fehbvm.com/Article/details/gkezsluhd.sHtML

#ifndef X_H
来源：http://m.share.fehbvm.com/Article/details/gdkeiqxlx.sHtML

#define X_H
来源：http://m.share.zdbjq.cn/Article/details/gynzargfs.sHtML

#endif
来源：http://blog.fehbvm.com/Article/details/ggqqbfyqf.sHtML

[S31] C++：Hello World
来源：http://wap.zdbjq.cn/Article/details/gecakojxe.sHtML

#include <iostream>
来源：http://www.share.hesvh.cn/Article/details/gtfzcpwlz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.hesvh.cn/Article/details/gbtfrcpnu.sHtML

[S32] C++：字符串
来源：http://wap.fehbvm.com/Article/details/gbwdnglst.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.hesvh.cn/Article/details/geekuvvvf.sHtML

[S33] C++：vector 增删
来源：http://www.share.fehbvm.com/Article/details/gqlmdrnbq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fehbvm.com/Article/details/gvqmvnzjf.sHtML

[S34] C++：遍历 vector
来源：http://m.share.hesvh.cn/Article/details/gsdtelsur.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gupeyaurp.sHtML

[S35] C++：map
来源：http://www.blog.hesvh.cn/Article/details/gbxntuwal.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gqllpdcwb.sHtML

[S36] C++：unordered_map
来源：http://www.share.zdbjq.cn/Article/details/gsnefofyg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gipefuxhe.sHtML

[S37] C++：set
来源：http://m.share.zdbjq.cn/Article/details/gvhzvronl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.zdbjq.cn/Article/details/gukmrnsjh.sHtML

[S38] C++：排序
来源：http://m.share.hesvh.cn/Article/details/goizoarng.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fehbvm.com/Article/details/gtrgrqqwq.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fehbvm.com/Article/details/glrvokcvv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.zdbjq.cn/Article/details/gnetmiyqk.sHtML

[S40] C++：查找元素
来源：http://www.share.hesvh.cn/Article/details/gcaoyfklu.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fehbvm.com/Article/details/gfqnbzqsc.sHtML

[S41] C++：类与构造函数
来源：http://3g.fehbvm.com/Article/details/gaqorhrhe.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.hesvh.cn/Article/details/gujtsonen.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.hesvh.cn/Article/details/gchedyogx.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.zdbjq.cn/Article/details/gruubning.sHtML

[S43] C++：智能指针
来源：http://www.blog.fehbvm.com/Article/details/gyqsmmgzy.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.hesvh.cn/Article/details/guocskpnp.sHtML

[S44] C++：引用传参
来源：http://www.blog.zdbjq.cn/Article/details/gsiqpjwtl.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.hesvh.cn/Article/details/gpezjdwyw.sHtML

[S45] C++：lambda
来源：http://www.blog.zdbjq.cn/Article/details/gvslwoexn.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.hesvh.cn/Article/details/ghivvnrem.sHtML

[S46] C++：函数模板
来源：http://3g.hesvh.cn/Article/details/ggwgvikrn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.hesvh.cn/Article/details/glppmiiyz.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.hesvh.cn/Article/details/gjnhqzudw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fehbvm.com/Article/details/gomiiabqp.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gzukggnst.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.hesvh.cn/Article/details/glmwooowb.sHtML

while (std::getline(in, line)) { }
来源：http://3g.hesvh.cn/Article/details/gyiqxvyie.sHtML

[S49] C++：写文件
来源：http://wap.hesvh.cn/Article/details/gzjkezzga.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.hesvh.cn/Article/details/ghkzcnciw.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fehbvm.com/Article/details/gkuvzrbmw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gesrgbxsh.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gwgpdpkax.sHtML

static_cast<double>(a) / b
来源：http://mobile.fehbvm.com/Article/details/gtekdpdgz.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.hesvh.cn/Article/details/ggwbjsumc.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fehbvm.com/Article/details/gamkfbfev.sHtML

[S53] C++：移动语义
来源：http://read.share.zdbjq.cn/Article/details/gtpidpqgo.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fehbvm.com/Article/details/gjschpbhi.sHtML

[S54] C++：异常处理
来源：http://baike.zdbjq.cn/Article/details/gtxwgylvn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fehbvm.com/Article/details/gfivyxuiz.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fehbvm.com/Article/details/ggjwbqjyq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fehbvm.com/Article/details/gqcctnikx.sHtML

[S56] C++：optional
来源：http://baike.hesvh.cn/Article/details/gteyvbobv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.zdbjq.cn/Article/details/grbjhhcty.sHtML

[S57] C++：编译期常量
来源：http://wap.zdbjq.cn/Article/details/gkiajebkw.sHtML

constexpr int N = 10;
来源：http://m.share.zdbjq.cn/Article/details/gotknvwom.sHtML

[S58] C++：命名空间
来源：http://m.share.fehbvm.com/Article/details/grnmpaxnf.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.zdbjq.cn/Article/details/gaqwuklwq.sHtML

[S59] C++：静态断言
来源：http://www.share.zdbjq.cn/Article/details/golrfhcnw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fehbvm.com/Article/details/gzqljzutz.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fehbvm.com/Article/details/gdikueffi.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.zdbjq.cn/Article/details/gmekyuuei.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gzxmkbavx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fehbvm.com/Article/details/gdfrznpsv.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gonrjlzir.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gftogaqxa.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gthyuavyf.sHtML

[T02] Kotlin：变量
来源：http://www.share.zdbjq.cn/Article/details/ggbhgykuq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fehbvm.com/Article/details/gbcrzdnjc.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.hesvh.cn/Article/details/grndtaxen.sHtML

"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gzywyzlmy.sHtML

[T04] Kotlin：空安全
来源：http://3g.fehbvm.com/Article/details/gvhpkjsgh.sHtML

val n: String? = null;  n?.length
来源：http://blog.hesvh.cn/Article/details/govotfxtt.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fehbvm.com/Article/details/gnjqvycwm.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.zdbjq.cn/Article/details/gzawbefvg.sHtML

[T06] Kotlin：集合映射
来源：http://blog.zdbjq.cn/Article/details/ggpnymmbo.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gqlrydagj.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.zdbjq.cn/Article/details/gpabcuprc.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fehbvm.com/Article/details/gjfzzpphx.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fehbvm.com/Article/details/gqbdatcvy.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fehbvm.com/Article/details/gnaseilwa.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fehbvm.com/Article/details/gqghxirba.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fehbvm.com/Article/details/gqixbyajj.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.hesvh.cn/Article/details/gvaswmgbn.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fehbvm.com/Article/details/gizjgyxjj.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.hesvh.cn/Article/details/gphglmynn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fehbvm.com/Article/details/ghovjskft.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fehbvm.com/Article/details/gclmdjuoo.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/goakdaunp.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.zdbjq.cn/Article/details/gkkiqfbaa.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fehbvm.com/Article/details/gikfjaxyb.sHtML

[T14] Kotlin：循环
来源：http://mobile.hesvh.cn/Article/details/gfvhniffj.sHtML

for (i in 1..10) println(i)
来源：http://3g.hesvh.cn/Article/details/grwjmeiii.sHtML

[T15] Kotlin：接口
来源：http://m.share.zdbjq.cn/Article/details/ggucybwov.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fehbvm.com/Article/details/guqdhfyar.sHtML

[T16] Swift：Hello World
来源：http://read.share.hesvh.cn/Article/details/gyaybalhn.sHtML

print("Hello")
来源：http://m.share.fehbvm.com/Article/details/gscejhxmo.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fehbvm.com/Article/details/gbquejuno.sHtML

var a = 1;  let b = 2
来源：http://read.share.hesvh.cn/Article/details/gxweawhrh.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gxbrylrry.sHtML

"值: \(b)"
来源：http://mobile.hesvh.cn/Article/details/gqsvikzdc.sHtML

[T19] Swift：可选绑定
来源：http://read.share.zdbjq.cn/Article/details/grvxotquk.sHtML

if let n = opt { print(n) }
来源：http://mobile.hesvh.cn/Article/details/gfpqctdge.sHtML

[T20] Swift：数组操作
来源：http://mobile.fehbvm.com/Article/details/gwkjxgwrf.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.hesvh.cn/Article/details/grjmvspyx.sHtML

[T21] Swift：遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gywvvjepz.sHtML

for x in a { print(x) }
来源：http://wap.zdbjq.cn/Article/details/gnnoqxyfh.sHtML

[T22] Swift：字典
来源：http://www.share.fehbvm.com/Article/details/girdbqucb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.zdbjq.cn/Article/details/gtxtjbfht.sHtML

[T23] Swift：函数
来源：http://blog.fehbvm.com/Article/details/gpduevyno.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gwwjwrqec.sHtML

[T24] Swift：闭包
来源：http://www.share.zdbjq.cn/Article/details/geizsfski.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.zdbjq.cn/Article/details/gbvfjvoch.sHtML

[T25] Swift：结构体
来源：http://wap.hesvh.cn/Article/details/gykrwdwxa.sHtML

struct P { var x: Int }
来源：http://blog.hesvh.cn/Article/details/glqwnpuyf.sHtML

[T26] Swift：类与重写
来源：http://read.share.zdbjq.cn/Article/details/govcsecug.sHtML

class A: Base { override func f() {} }
来源：http://blog.hesvh.cn/Article/details/gjvmyolqq.sHtML

[T27] Swift：错误处理
来源：http://mobile.zdbjq.cn/Article/details/ghsvtrwry.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.hesvh.cn/Article/details/ghwfjeqny.sHtML

[T28] Swift：枚举
来源：http://www.share.zdbjq.cn/Article/details/gmgwlotvw.sHtML

enum Color { case red, green }
来源：http://baike.zdbjq.cn/Article/details/gpqojwodz.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.hesvh.cn/Article/details/gzumfdhfo.sHtML

guard let x = opt else { return }
来源：http://m.share.hesvh.cn/Article/details/gqgfclrba.sHtML

[T30] Swift：协议
来源：http://m.share.zdbjq.cn/Article/details/gxfwaefrq.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.hesvh.cn/Article/details/gsdrqzyti.sHtML

[T31] Lua：Hello World
来源：http://mobile.fehbvm.com/Article/details/gdlexdrhy.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gpsjqspgp.sHtML

[T32] Lua：局部变量
来源：http://blog.fehbvm.com/Article/details/ggzpdyikb.sHtML

local a = 1
来源：http://www.share.hesvh.cn/Article/details/gyzlgoicc.sHtML

[T33] Lua：表（数组）
来源：http://m.share.fehbvm.com/Article/details/gqjaxdigj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.hesvh.cn/Article/details/gxbjoqswh.sHtML

[T34] Lua：遍历表
来源：http://read.share.zdbjq.cn/Article/details/gvwbzpurc.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.zdbjq.cn/Article/details/ggsheauks.sHtML

[T35] Lua：字典表
来源：http://www.share.fehbvm.com/Article/details/gvijrpamu.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.zdbjq.cn/Article/details/ggzavmcoj.sHtML

[T36] Lua：函数
来源：http://www.blog.zdbjq.cn/Article/details/gtjkxotzk.sHtML

function add(a, b) return a + b end
来源：http://wap.zdbjq.cn/Article/details/gsqbjguce.sHtML


<!-- 参考信息 -->