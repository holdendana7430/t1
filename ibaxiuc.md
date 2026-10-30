代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fanxiaobao.xyz/Article/details/gsmmzxjwa.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggjixnpmb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fanxiaobao.xyz/Article/details/guoybreag.sHtML

[R37] 把输出赋给变量
来源：http://baike.fanxiaobao.xyz/Article/details/gdbmdpjqn.sHtML

files=$(ls -1)
来源：http://wap.fanxiaobao.xyz/Article/details/goizewbpe.sHtML

[R38] 管道串联
来源：http://3g.fanxiaobao.xyz/Article/details/gypxiavzp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyqkdxebq.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fanxiaobao.xyz/Article/details/glkizklbg.sHtML

cmd > out.log 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gvkqqitay.sHtML

[R40] 追加写日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gzyoqpyfz.sHtML

echo "log" >> out.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gafhcylal.sHtML

[R41] 丢弃输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gxkhjnyme.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gghlnfcvt.sHtML

[R42] 输入重定向
来源：http://mobile.fanxiaobao.xyz/Article/details/ggnquknjh.sHtML

wc -l < a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/ghcnehvzf.sHtML

[R43] 按名字查找文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gnsyvdkla.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gzfggsfii.sHtML

[R44] 按修改时间查找
来源：http://3g.fanxiaobao.xyz/Article/details/gcvlscvmv.sHtML

find . -mtime -7 -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/goydulgws.sHtML

[R45] 批量删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gfpxullai.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fanxiaobao.xyz/Article/details/gymycywlj.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fanxiaobao.xyz/Article/details/gppjxegnv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxaitmra.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gstaxbtry.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gupdagjrv.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gqyhqhxlm.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gslwcbmji.sHtML

[R49] awk 带条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gjaeqodnb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fanxiaobao.xyz/Article/details/gzsnuyylb.sHtML

[R50] awk 求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gfnbkelpd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gihjuyzej.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gedhihxay.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fanxiaobao.xyz/Article/details/gmjbedhoz.sHtML

[R52] 统计行数
来源：http://m.share.fanxiaobao.xyz/Article/details/gsdluppkv.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gxscifcwv.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtscpojgd.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fanxiaobao.xyz/Article/details/grjqkxpyh.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/guhywvdoe.sHtML

diff a.txt b.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gzfdfokua.sHtML

[R55] 压缩与解压
来源：http://3g.fanxiaobao.xyz/Article/details/gbqoxvubu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guokpjugx.sHtML

[R56] 远程拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gotvtqufu.sHtML

scp file user@host:/path/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxnrdodqq.sHtML

[R57] 远程执行命令
来源：http://3g.fanxiaobao.xyz/Article/details/gfulzeuad.sHtML

ssh user@host 'uptime'
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxcfiljv.sHtML

[R58] 下载文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gjsahqtdw.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gahompnjn.sHtML

[R59] 发 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gczgaheki.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fanxiaobao.xyz/Article/details/glzkraztf.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gwhsnwfrk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fanxiaobao.xyz/Article/details/gsdfahajg.sHtML

[R61] 磁盘占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghxodmffg.sHtML

df -h;  du -sh *
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyjstksay.sHtML

[R62] 找最占空间的文件
来源：http://wap.fanxiaobao.xyz/Article/details/gvltfmwgi.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fanxiaobao.xyz/Article/details/gwfsojhzw.sHtML

[R63] 内存与进程
来源：http://wap.fanxiaobao.xyz/Article/details/gitugkdiz.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglohwjzd.sHtML

[R64] 结束进程
来源：http://blog.fanxiaobao.xyz/Article/details/gosbmqlnt.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzgbkjhiz.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdchbcyzg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxkggahq.sHtML

[R66] 定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gdfgbmlis.sHtML

crontab -e;  crontab -l
来源：http://m.share.fanxiaobao.xyz/Article/details/ghltgirqc.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fanxiaobao.xyz/Article/details/gicvqqbaf.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/gqilnogux.sHtML

[R68] 计算文件校验值
来源：http://read.share.fanxiaobao.xyz/Article/details/gorctiqpx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/ghbfqmcnv.sHtML

[R69] 生成随机密码
来源：http://read.share.fanxiaobao.xyz/Article/details/guryzwkbu.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/gfivyzrsr.sHtML

[R70] 时间戳与互转
来源：http://mobile.fanxiaobao.xyz/Article/details/gmqyjqcze.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fanxiaobao.xyz/Article/details/gifgnxlmi.sHtML

[R71] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gslegzlgk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fanxiaobao.xyz/Article/details/ggcocixml.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/gzideucht.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtokgvrkp.sHtML

[R73] 分割大日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpononxhh.sHtML

split -l 1000 big.log part_
来源：http://www.share.fanxiaobao.xyz/Article/details/grjvfyrmu.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giwqveefa.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gsiueaobo.sHtML

[R75] 导出环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/grigrecuo.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fanxiaobao.xyz/Article/details/gfjwrqztb.sHtML

[R76] 使用临时文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gghmlgqwf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gzphmnfzc.sHtML

[R77] 读取用户输入
来源：http://m.share.fanxiaobao.xyz/Article/details/glppzwryg.sHtML

read -rp "请输入: " ans
来源：http://baike.fanxiaobao.xyz/Article/details/gmtqsgach.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/gwkiywyaj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fanxiaobao.xyz/Article/details/gdswicrpc.sHtML

[R79] 解析命令行选项
来源：http://mobile.fanxiaobao.xyz/Article/details/grgtytllg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdrsjnuu.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fanxiaobao.xyz/Article/details/gftbvtaah.sHtML

time ./run.sh
来源：http://baike.fanxiaobao.xyz/Article/details/gkxshcpjd.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gzdkypkpl.sHtML

S. C / C++ 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gkvrtqsvj.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gctxrruqb.sHtML

[S01] C：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gcaevtbmz.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/gyekifxim.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwriitpum.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fanxiaobao.xyz/Article/details/gqkrdyaqc.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fanxiaobao.xyz/Article/details/grbbblcju.sHtML

[S03] C：读入整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmkxjbozk.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqycpwsik.sHtML

[S04] C：字符串复制
来源：http://m.share.fanxiaobao.xyz/Article/details/gbkkzlsme.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/gptyqrpcb.sHtML

[S05] C：字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/guuwgtacq.sHtML

strlen(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gdvmtnzdr.sHtML

[S06] C：字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/goowqhxsv.sHtML

strcmp(a, b) == 0
来源：http://blog.fanxiaobao.xyz/Article/details/gpjsshhxo.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcpcwaeby.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gccrfhioj.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fanxiaobao.xyz/Article/details/gvtdxiclf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdbutqso.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fanxiaobao.xyz/Article/details/gsmtcsazs.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/geqhzwdub.sHtML

[S10] C：指针与解引用
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxfiypvv.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvlezqxgl.sHtML

[S11] C：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gyqgmeicf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fanxiaobao.xyz/Article/details/gobadmezg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdqybyptn.sHtML

fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/ghhpotzfp.sHtML

[S12] C：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gzslsvsnm.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gisohtqme.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gghhzpkjh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fanxiaobao.xyz/Article/details/girdmkdke.sHtML

[S14] C：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gvcaxudzj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcceratqu.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdgxrvps.sHtML

(double) a / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqfqmsfaa.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/grhvvktqk.sHtML

x |= (1 << 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/grupfbcxo.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gjropgcyt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fanxiaobao.xyz/Article/details/glcshjkax.sHtML

[S18] C：命令行参数
来源：http://wap.fanxiaobao.xyz/Article/details/gdtmvkzpt.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghiezpiby.sHtML

[S19] C：快速排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmwvniuy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxzsqcyr.sHtML

[S20] C：二分查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbhjbqxn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/grftxsdrp.sHtML

[S21] C：字符类别判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gjrebkoiu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkmussjdd.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmaoedwtn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdqeiimfv.sHtML

[S23] C：随机数
来源：http://www.share.fanxiaobao.xyz/Article/details/gdnbvykyt.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gwvfcmauv.sHtML

[S24] C：获取本地时间
来源：http://blog.fanxiaobao.xyz/Article/details/gxppuyrna.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fanxiaobao.xyz/Article/details/gegjqavrc.sHtML

[S25] C：内存拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/goeslddze.sHtML

memcpy(dst, src, n);
来源：http://baike.fanxiaobao.xyz/Article/details/gdqffpjwy.sHtML

[S26] C：内存清零
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpkjxkrem.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fanxiaobao.xyz/Article/details/gbnrpsosw.sHtML

[S27] C：定义常量
来源：http://baike.fanxiaobao.xyz/Article/details/gqahnqpfn.sHtML

const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gefedddzc.sHtML

[S28] C：静态变量
来源：http://3g.fanxiaobao.xyz/Article/details/gtfcfmtpd.sHtML

static int counter = 0;
来源：http://wap.fanxiaobao.xyz/Article/details/gilknjoyc.sHtML

[S29] C：变参函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gezbloace.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fanxiaobao.xyz/Article/details/guwwekikh.sHtML

[S30] C：头文件保护
来源：http://3g.fanxiaobao.xyz/Article/details/gnetqhtij.sHtML

#ifndef X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzdicmmz.sHtML

#define X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhvxhxgh.sHtML

#endif
来源：http://read.share.fanxiaobao.xyz/Article/details/gkmgygtxq.sHtML

[S31] C++：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gpvnpdcdv.sHtML

#include <iostream>
来源：http://baike.fanxiaobao.xyz/Article/details/gbdkujxzk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gqyqrhjwq.sHtML

[S32] C++：字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gayznqfuz.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fanxiaobao.xyz/Article/details/gtbfyhfep.sHtML

[S33] C++：vector 增删
来源：http://baike.fanxiaobao.xyz/Article/details/gdabhjnfr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/glopzarrq.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fanxiaobao.xyz/Article/details/gnlmsnyhi.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gyviagcos.sHtML

[S35] C++：map
来源：http://m.share.fanxiaobao.xyz/Article/details/gfdazippr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/graegboss.sHtML

[S36] C++：unordered_map
来源：http://mobile.fanxiaobao.xyz/Article/details/glcnkvxie.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gjmomvdpa.sHtML

[S37] C++：set
来源：http://mobile.fanxiaobao.xyz/Article/details/gfghwntcf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gzsrjuprd.sHtML

[S38] C++：排序
来源：http://wap.fanxiaobao.xyz/Article/details/gqavlwocz.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/ghilvbzdl.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fanxiaobao.xyz/Article/details/gxvjwrxqh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fanxiaobao.xyz/Article/details/gvoeinsbc.sHtML

[S40] C++：查找元素
来源：http://baike.fanxiaobao.xyz/Article/details/glqvgvnfe.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmtpljvva.sHtML

[S41] C++：类与构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/gidvaapme.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/getjkvgrh.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gftikjtme.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fanxiaobao.xyz/Article/details/glubcvslt.sHtML

[S43] C++：智能指针
来源：http://3g.fanxiaobao.xyz/Article/details/gyzqilyqw.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fanxiaobao.xyz/Article/details/glmfcdoyp.sHtML

[S44] C++：引用传参
来源：http://read.share.fanxiaobao.xyz/Article/details/gamabhspb.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gglvaomrg.sHtML

[S45] C++：lambda
来源：http://baike.fanxiaobao.xyz/Article/details/gcmuizpgm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fanxiaobao.xyz/Article/details/giddpvaex.sHtML

[S46] C++：函数模板
来源：http://wap.fanxiaobao.xyz/Article/details/gbgtqvtiz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fanxiaobao.xyz/Article/details/ghhdujgar.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqluszhjj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkxfctzos.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefcylsml.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fanxiaobao.xyz/Article/details/guxmpzxat.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbcbdphgl.sHtML

[S49] C++：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gaytmqhav.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjvsuepx.sHtML

[S50] C++：格式化数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtpxazty.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gojmrggfn.sHtML

[S51] C++：显式类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gfxmaetqw.sHtML

static_cast<double>(a) / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfuuwcxr.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fanxiaobao.xyz/Article/details/gxyjwpzjd.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fanxiaobao.xyz/Article/details/gcouwqgen.sHtML

[S53] C++：移动语义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcstlktpa.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fanxiaobao.xyz/Article/details/gwxmctath.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmobrddkl.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqqsycpt.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzkbpoqua.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fanxiaobao.xyz/Article/details/glaiozpob.sHtML

[S56] C++：optional
来源：http://m.share.fanxiaobao.xyz/Article/details/gohrsadxo.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fanxiaobao.xyz/Article/details/gmkcdjxhv.sHtML

[S57] C++：编译期常量
来源：http://blog.fanxiaobao.xyz/Article/details/gqkzvgnel.sHtML

constexpr int N = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glepicpci.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvdzwobzs.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/guvofhswd.sHtML

[S59] C++：静态断言
来源：http://www.share.fanxiaobao.xyz/Article/details/gcsfjllyw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fanxiaobao.xyz/Article/details/gdjxknuiu.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gplvdicmw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gegtjtcrt.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grlifksbs.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fanxiaobao.xyz/Article/details/gezngmfas.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gdjjwfhtj.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gyqtbwmsk.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gbeqvyksd.sHtML

[T02] Kotlin：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gnovkuezk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fanxiaobao.xyz/Article/details/gevafyuni.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fanxiaobao.xyz/Article/details/geybbzfxt.sHtML

"值: $b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gggioxvhe.sHtML

[T04] Kotlin：空安全
来源：http://wap.fanxiaobao.xyz/Article/details/gzfwtxptx.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhygfafn.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gjawobsir.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fanxiaobao.xyz/Article/details/gzotczlae.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/goeuyisja.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/gxcqwlhpc.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/ggdsbaixa.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmwdvwal.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gypjtqovw.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/goatxjkxh.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcflmlptl.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fanxiaobao.xyz/Article/details/guhukocym.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtfnykfzo.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fanxiaobao.xyz/Article/details/gowzoqkat.sHtML

[T11] Kotlin：协程
来源：http://blog.fanxiaobao.xyz/Article/details/gahtenzcu.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqbernyij.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fanxiaobao.xyz/Article/details/gptpfebpy.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmxmtxfsd.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fanxiaobao.xyz/Article/details/gwhjiiqxw.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnxtgqeup.sHtML

[T14] Kotlin：循环
来源：http://3g.fanxiaobao.xyz/Article/details/gfnbifyxj.sHtML

for (i in 1..10) println(i)
来源：http://baike.fanxiaobao.xyz/Article/details/gjasnexmu.sHtML

[T15] Kotlin：接口
来源：http://read.share.fanxiaobao.xyz/Article/details/gobffuuwk.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghiohfayc.sHtML

[T16] Swift：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gqxncbogj.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxugpjbhj.sHtML

[T17] Swift：变量与常量
来源：http://blog.fanxiaobao.xyz/Article/details/gknxicdrz.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdhbindzf.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gywqbxvht.sHtML

"值: \(b)"
来源：http://m.share.fanxiaobao.xyz/Article/details/gtekvvgiz.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcrotzxpy.sHtML

if let n = opt { print(n) }
来源：http://blog.fanxiaobao.xyz/Article/details/gfcdhrqdn.sHtML

[T20] Swift：数组操作
来源：http://baike.fanxiaobao.xyz/Article/details/gphtxdrjb.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqjbiiwfr.sHtML

[T21] Swift：遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gfifykfwc.sHtML

for x in a { print(x) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwsmrqruz.sHtML

[T22] Swift：字典
来源：http://wap.fanxiaobao.xyz/Article/details/gtibbzjbf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gnrwpvpik.sHtML

[T23] Swift：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/guxfnvahj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfoyymtca.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmfmpfca.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/geeenruur.sHtML

[T25] Swift：结构体
来源：http://3g.fanxiaobao.xyz/Article/details/gqmqzjctl.sHtML

struct P { var x: Int }
来源：http://baike.fanxiaobao.xyz/Article/details/gkydqjrei.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzcrhzfyx.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtpvivzhu.sHtML

[T27] Swift：错误处理
来源：http://wap.fanxiaobao.xyz/Article/details/gdiajzchx.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzyececkm.sHtML

[T28] Swift：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gllnjtocr.sHtML

enum Color { case red, green }
来源：http://wap.fanxiaobao.xyz/Article/details/gdzdtszoi.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghbqfnjy.sHtML

guard let x = opt else { return }
来源：http://blog.fanxiaobao.xyz/Article/details/gtjfbihyc.sHtML

[T30] Swift：协议
来源：http://blog.fanxiaobao.xyz/Article/details/gegrqrxiz.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/gukykwbpg.sHtML

[T31] Lua：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gafrqhtdj.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/guhznqsyg.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajcndctq.sHtML

local a = 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gpysjmerj.sHtML

[T33] Lua：表（数组）
来源：http://baike.fanxiaobao.xyz/Article/details/gqideblvn.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fanxiaobao.xyz/Article/details/gksirudjj.sHtML

[T34] Lua：遍历表
来源：http://baike.fanxiaobao.xyz/Article/details/gqsphdlay.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.fanxiaobao.xyz/Article/details/geogomfld.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwejrpby.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtubtgyuv.sHtML

[T36] Lua：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gnqjybchh.sHtML

function add(a, b) return a + b end
来源：http://www.share.fanxiaobao.xyz/Article/details/gdrconijh.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/gfnnlbjys.sHtML

"a" .. "b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gsrnfshpa.sHtML

[T38] Lua：条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gsrzuhrbb.sHtML

if x > 0 then print("正") end
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhkawpme.sHtML


<!-- 参考信息 -->