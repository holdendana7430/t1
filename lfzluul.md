代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://m.share.hesvh.cn/Article/details/gciuppdxb.sHtML

[R32] 参数个数校验
来源：http://blog.hesvh.cn/Article/details/gastianlz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/gsaodrlua.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fehbvm.com/Article/details/grnrxytjl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.hesvh.cn/Article/details/gvvhgkfvf.sHtML

[R34] 退出时清理
来源：http://baike.fehbvm.com/Article/details/gicdqkjah.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/ghkatayyx.sHtML

[R35] 后台执行并等待
来源：http://baike.zdbjq.cn/Article/details/goeafvcjc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fehbvm.com/Article/details/guwzgwctu.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fehbvm.com/Article/details/gsiakoabb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.hesvh.cn/Article/details/girsxwbar.sHtML

[R37] 把输出赋给变量
来源：http://www.share.hesvh.cn/Article/details/gxvftvfvj.sHtML

files=$(ls -1)
来源：http://www.blog.zdbjq.cn/Article/details/gqazdzuzi.sHtML

[R38] 管道串联
来源：http://wap.fehbvm.com/Article/details/gtreodnwy.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.hesvh.cn/Article/details/gwptqaqon.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.zdbjq.cn/Article/details/gdivvsgqc.sHtML

cmd > out.log 2>&1
来源：http://mobile.hesvh.cn/Article/details/gcfnejdft.sHtML

[R40] 追加写日志
来源：http://wap.fehbvm.com/Article/details/gnfnrchic.sHtML

echo "log" >> out.log
来源：http://www.share.zdbjq.cn/Article/details/gbquwgumu.sHtML

[R41] 丢弃输出
来源：http://baike.hesvh.cn/Article/details/glkkzhshv.sHtML

cmd >/dev/null 2>&1
来源：http://baike.hesvh.cn/Article/details/gwhnfwske.sHtML

[R42] 输入重定向
来源：http://www.share.zdbjq.cn/Article/details/gzqvyqjbh.sHtML

wc -l < a.txt
来源：http://www.blog.fehbvm.com/Article/details/guwdjozga.sHtML

[R43] 按名字查找文件
来源：http://3g.fehbvm.com/Article/details/gqafmhrxg.sHtML

find . -name "*.log" -type f
来源：http://3g.zdbjq.cn/Article/details/gjiqlhuoi.sHtML

[R44] 按修改时间查找
来源：http://3g.fehbvm.com/Article/details/gbnfgcoyt.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fehbvm.com/Article/details/gqahjirkr.sHtML

[R45] 批量删除
来源：http://read.share.hesvh.cn/Article/details/glpbsrgcu.sHtML

find . -name "*.tmp" -delete
来源：http://blog.hesvh.cn/Article/details/ggmeevbgg.sHtML

[R46] 递归替换文件内容
来源：http://blog.fehbvm.com/Article/details/gdmjjypbn.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.hesvh.cn/Article/details/gamemwugv.sHtML

[R47] sed 单行替换
来源：http://m.share.fehbvm.com/Article/details/gplfnulms.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fehbvm.com/Article/details/ghuzadqiz.sHtML

[R48] awk 取指定列
来源：http://www.share.fehbvm.com/Article/details/gfjzfyqde.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fehbvm.com/Article/details/gsbasrssn.sHtML

[R49] awk 带条件
来源：http://www.share.hesvh.cn/Article/details/gzcetqqsz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.hesvh.cn/Article/details/gjzidubkk.sHtML

[R50] awk 求和
来源：http://mobile.zdbjq.cn/Article/details/gtlkjpttj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fehbvm.com/Article/details/gyofdavvi.sHtML

[R51] 排序去重取前几
来源：http://3g.fehbvm.com/Article/details/gpcvzzjiy.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fehbvm.com/Article/details/gtigtpoav.sHtML

[R52] 统计行数
来源：http://baike.hesvh.cn/Article/details/gcuqsacao.sHtML

wc -l a.txt
来源：http://m.share.hesvh.cn/Article/details/gwuizggxz.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fehbvm.com/Article/details/ghwgwtvig.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.hesvh.cn/Article/details/gbodflgwj.sHtML

[R54] 比较两个文件
来源：http://mobile.hesvh.cn/Article/details/gyuuxpbdt.sHtML

diff a.txt b.txt
来源：http://m.share.hesvh.cn/Article/details/gskeuvsmq.sHtML

[R55] 压缩与解压
来源：http://baike.fehbvm.com/Article/details/ghpyrfbbp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.hesvh.cn/Article/details/gheztuujz.sHtML

[R56] 远程拷贝
来源：http://read.share.hesvh.cn/Article/details/grslspzor.sHtML

scp file user@host:/path/
来源：http://read.share.zdbjq.cn/Article/details/gsatxdgan.sHtML

[R57] 远程执行命令
来源：http://www.m.share.hesvh.cn/Article/details/gbszqwzyg.sHtML

ssh user@host 'uptime'
来源：http://www.share.fehbvm.com/Article/details/gipidtzny.sHtML

[R58] 下载文件
来源：http://3g.fehbvm.com/Article/details/gjyiqstbz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fehbvm.com/Article/details/gatlkhqie.sHtML

[R59] 发 POST JSON
来源：http://wap.fehbvm.com/Article/details/gsbcmhfsn.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.zdbjq.cn/Article/details/goybvpyrq.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/gsgttacax.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fehbvm.com/Article/details/gdppdjnby.sHtML

[R61] 磁盘占用
来源：http://m.share.zdbjq.cn/Article/details/gxzphiuaz.sHtML

df -h;  du -sh *
来源：http://baike.zdbjq.cn/Article/details/golsvjshc.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.hesvh.cn/Article/details/gkhyjgxoq.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.zdbjq.cn/Article/details/gseuyujmf.sHtML

[R63] 内存与进程
来源：http://www.blog.hesvh.cn/Article/details/gtzxdszsn.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.hesvh.cn/Article/details/gmdfxbkup.sHtML

[R64] 结束进程
来源：http://3g.fehbvm.com/Article/details/gmkpqgyth.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.zdbjq.cn/Article/details/gfioucqxe.sHtML

[R65] 查看端口占用
来源：http://blog.zdbjq.cn/Article/details/gqwkzrhto.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.zdbjq.cn/Article/details/gnoctehvf.sHtML

[R66] 定时任务
来源：http://m.share.zdbjq.cn/Article/details/gxqlkxeyz.sHtML

crontab -e;  crontab -l
来源：http://baike.fehbvm.com/Article/details/gxwfdxxfj.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.zdbjq.cn/Article/details/gccfuuczq.sHtML

openssl rand -hex 16
来源：http://www.blog.zdbjq.cn/Article/details/gbdihddqy.sHtML

[R68] 计算文件校验值
来源：http://www.blog.zdbjq.cn/Article/details/glmwxnfbq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.hesvh.cn/Article/details/gevrzfvnk.sHtML

[R69] 生成随机密码
来源：http://wap.fehbvm.com/Article/details/gnwdxpens.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.zdbjq.cn/Article/details/glkjjkwlk.sHtML

[R70] 时间戳与互转
来源：http://read.share.zdbjq.cn/Article/details/ggmhutgmi.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.hesvh.cn/Article/details/grcyydcoj.sHtML

[R71] 日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/ggahgpffe.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fehbvm.com/Article/details/grifrvzui.sHtML

[R72] 等待端口就绪
来源：http://www.blog.hesvh.cn/Article/details/glajnkleg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gxtgfmvsd.sHtML

[R73] 分割大日志
来源：http://m.share.hesvh.cn/Article/details/gzinvafmb.sHtML

split -l 1000 big.log part_
来源：http://www.blog.zdbjq.cn/Article/details/ggnmibmfk.sHtML

[R74] 批量重命名
来源：http://www.m.share.hesvh.cn/Article/details/gtynqcpan.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.hesvh.cn/Article/details/gdzilghfl.sHtML

[R75] 导出环境变量
来源：http://blog.hesvh.cn/Article/details/gqjfffraz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.zdbjq.cn/Article/details/gmolkmzof.sHtML

[R76] 使用临时文件
来源：http://mobile.zdbjq.cn/Article/details/gnydervnl.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gpzscpwzy.sHtML

[R77] 读取用户输入
来源：http://www.blog.zdbjq.cn/Article/details/gkhcqwjwe.sHtML

read -rp "请输入: " ans
来源：http://www.blog.hesvh.cn/Article/details/gjvmkcqtn.sHtML

[R78] 交互式菜单
来源：http://www.m.share.zdbjq.cn/Article/details/gaaydkmta.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.hesvh.cn/Article/details/golbkocfq.sHtML

[R79] 解析命令行选项
来源：http://blog.fehbvm.com/Article/details/gkdoizcus.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.zdbjq.cn/Article/details/giuuafdef.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fehbvm.com/Article/details/glrrmyetb.sHtML

time ./run.sh
来源：http://m.share.fehbvm.com/Article/details/gombovtbr.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gflvzllml.sHtML

S. C / C++ 专题
来源：http://wap.zdbjq.cn/Article/details/gbmzgrobm.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gwprshvzf.sHtML

[S01] C：Hello World
来源：http://baike.fehbvm.com/Article/details/gqoalqqfs.sHtML

#include <stdio.h>
来源：http://www.share.hesvh.cn/Article/details/gcyfrpuzi.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.hesvh.cn/Article/details/gwratbygq.sHtML

[S02] C：变量与格式化输出
来源：http://blog.hesvh.cn/Article/details/gtqjbllpt.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fehbvm.com/Article/details/gfhnnsugg.sHtML

[S03] C：读入整数
来源：http://baike.fehbvm.com/Article/details/gytjlaxim.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.zdbjq.cn/Article/details/gwuxqrwsw.sHtML

[S04] C：字符串复制
来源：http://blog.fehbvm.com/Article/details/gghuikout.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fehbvm.com/Article/details/gdfedapzg.sHtML

[S05] C：字符串长度
来源：http://m.share.hesvh.cn/Article/details/gukrtmuzh.sHtML

strlen(s)
来源：http://blog.zdbjq.cn/Article/details/gozugbopt.sHtML

[S06] C：字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gbzdqywib.sHtML

strcmp(a, b) == 0
来源：http://read.share.hesvh.cn/Article/details/gfmghmgjg.sHtML

[S07] C：数组遍历求和
来源：http://3g.hesvh.cn/Article/details/gqzwbuuiw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.hesvh.cn/Article/details/grawqdurn.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fehbvm.com/Article/details/gbrhnvzas.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.hesvh.cn/Article/details/gdemojzfb.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.hesvh.cn/Article/details/gydgdzhnc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.zdbjq.cn/Article/details/gszqovhys.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fehbvm.com/Article/details/gngkmwvqc.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.zdbjq.cn/Article/details/gmurmjvbe.sHtML

[S11] C：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gdqxwrdqa.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fehbvm.com/Article/details/gkwfmkprf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gyzngcmbl.sHtML

fclose(f);
来源：http://mobile.hesvh.cn/Article/details/ghhhrrcas.sHtML

[S12] C：写文件
来源：http://wap.zdbjq.cn/Article/details/gwkuzohlj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gwtksejmd.sHtML

[S13] C：宏定义
来源：http://mobile.fehbvm.com/Article/details/grupcbdjd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.zdbjq.cn/Article/details/grzbeavkk.sHtML

[S14] C：枚举
来源：http://www.share.fehbvm.com/Article/details/gyxohcyzv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.zdbjq.cn/Article/details/gkkfwnshk.sHtML

[S15] C：类型转换
来源：http://www.m.share.fehbvm.com/Article/details/gcfqfjpxw.sHtML

(double) a / b
来源：http://wap.hesvh.cn/Article/details/gnmktbiyv.sHtML

[S16] C：位操作置位
来源：http://www.share.zdbjq.cn/Article/details/ganlebcuz.sHtML

x |= (1 << 3);
来源：http://read.share.zdbjq.cn/Article/details/gfqdzidtl.sHtML

[S17] C：安全拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gngtybtvb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fehbvm.com/Article/details/gwwkhoeed.sHtML

[S18] C：命令行参数
来源：http://m.share.zdbjq.cn/Article/details/gpwvqtrxw.sHtML

int main(int argc, char **argv)
来源：http://www.blog.zdbjq.cn/Article/details/gojilhfas.sHtML

[S19] C：快速排序
来源：http://mobile.zdbjq.cn/Article/details/gcanlscgv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/gpuivjksl.sHtML

[S20] C：二分查找
来源：http://baike.fehbvm.com/Article/details/gyyxdhqtq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/gcilydqjv.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fehbvm.com/Article/details/glfejolak.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fehbvm.com/Article/details/ghooxbvbk.sHtML

[S22] C：字符串转数字
来源：http://m.share.zdbjq.cn/Article/details/gaqvvqozw.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.hesvh.cn/Article/details/gohgcuzhs.sHtML

[S23] C：随机数
来源：http://www.blog.zdbjq.cn/Article/details/ggmurlrvr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.zdbjq.cn/Article/details/gzngggivn.sHtML

[S24] C：获取本地时间
来源：http://baike.hesvh.cn/Article/details/grbfhvslg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fehbvm.com/Article/details/glhblqyfz.sHtML

[S25] C：内存拷贝
来源：http://wap.fehbvm.com/Article/details/gwciievlw.sHtML

memcpy(dst, src, n);
来源：http://m.share.fehbvm.com/Article/details/gwufvomgk.sHtML

[S26] C：内存清零
来源：http://baike.hesvh.cn/Article/details/gyeltmenn.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.zdbjq.cn/Article/details/gwoebyxfg.sHtML

[S27] C：定义常量
来源：http://www.blog.zdbjq.cn/Article/details/gvaygzcty.sHtML

const double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gosmtyxpe.sHtML

[S28] C：静态变量
来源：http://m.share.fehbvm.com/Article/details/govbefvsn.sHtML

static int counter = 0;
来源：http://mobile.fehbvm.com/Article/details/guzcnzjuf.sHtML

[S29] C：变参函数
来源：http://www.m.share.zdbjq.cn/Article/details/gifwqtesh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fehbvm.com/Article/details/glxknxwge.sHtML

[S30] C：头文件保护
来源：http://www.share.fehbvm.com/Article/details/gyxucuhyc.sHtML

#ifndef X_H
来源：http://www.blog.zdbjq.cn/Article/details/gklkhetjy.sHtML

#define X_H
来源：http://www.m.share.fehbvm.com/Article/details/gyixecdzs.sHtML

#endif
来源：http://m.share.zdbjq.cn/Article/details/gdlypeecu.sHtML

[S31] C++：Hello World
来源：http://www.share.zdbjq.cn/Article/details/ggnixayub.sHtML

#include <iostream>
来源：http://blog.hesvh.cn/Article/details/gsnggffmn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.hesvh.cn/Article/details/gsbpxvixe.sHtML

[S32] C++：字符串
来源：http://m.share.zdbjq.cn/Article/details/gslmabpvp.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.hesvh.cn/Article/details/gstorfywq.sHtML

[S33] C++：vector 增删
来源：http://mobile.fehbvm.com/Article/details/gtigmcmbv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fehbvm.com/Article/details/goezdlhql.sHtML

[S34] C++：遍历 vector
来源：http://mobile.hesvh.cn/Article/details/gcmasxvzb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.hesvh.cn/Article/details/grzrmwkeg.sHtML

[S35] C++：map
来源：http://www.share.fehbvm.com/Article/details/gbwxzwrfs.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gowdqiaqy.sHtML

[S36] C++：unordered_map
来源：http://mobile.fehbvm.com/Article/details/gzxwrbyqm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/gmpuwoyqd.sHtML

[S37] C++：set
来源：http://3g.hesvh.cn/Article/details/gdpphcstf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gmbccttrt.sHtML

[S38] C++：排序
来源：http://3g.fehbvm.com/Article/details/giazcibyp.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.zdbjq.cn/Article/details/gqnsbesxw.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.hesvh.cn/Article/details/giixmnnrh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.zdbjq.cn/Article/details/gtidqjwxv.sHtML

[S40] C++：查找元素
来源：http://read.share.fehbvm.com/Article/details/gdrashkmr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.zdbjq.cn/Article/details/ggholclnk.sHtML

[S41] C++：类与构造函数
来源：http://blog.hesvh.cn/Article/details/gjkvayemp.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.zdbjq.cn/Article/details/gzqrewdlc.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.zdbjq.cn/Article/details/gigixvsry.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.zdbjq.cn/Article/details/gotpzrssu.sHtML

[S43] C++：智能指针
来源：http://wap.hesvh.cn/Article/details/gsprhtsmw.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fehbvm.com/Article/details/glxqgnfrs.sHtML

[S44] C++：引用传参
来源：http://baike.fehbvm.com/Article/details/gdzluvsin.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.hesvh.cn/Article/details/gbmyxjyyh.sHtML

[S45] C++：lambda
来源：http://read.share.zdbjq.cn/Article/details/gpvsopqbb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.hesvh.cn/Article/details/gtvcxsaak.sHtML

[S46] C++：函数模板
来源：http://3g.hesvh.cn/Article/details/ggalsgxxz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.zdbjq.cn/Article/details/grzufcuze.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.hesvh.cn/Article/details/giwaxbhcz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.zdbjq.cn/Article/details/gikosveor.sHtML

[S48] C++：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gjzbbndbf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.zdbjq.cn/Article/details/gktzbaiku.sHtML

while (std::getline(in, line)) { }
来源：http://blog.hesvh.cn/Article/details/glvahuwgd.sHtML

[S49] C++：写文件
来源：http://mobile.zdbjq.cn/Article/details/glswftval.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.zdbjq.cn/Article/details/gqhirzqko.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.zdbjq.cn/Article/details/gshcghuci.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gghrifadc.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fehbvm.com/Article/details/gbmwjmatr.sHtML

static_cast<double>(a) / b
来源：http://m.share.fehbvm.com/Article/details/gyytujlur.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fehbvm.com/Article/details/gotxvgkbd.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fehbvm.com/Article/details/gzesuhyse.sHtML

[S53] C++：移动语义
来源：http://baike.fehbvm.com/Article/details/gcyjvivwd.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fehbvm.com/Article/details/gmjfeobry.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fehbvm.com/Article/details/gipztjwin.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.hesvh.cn/Article/details/gqslmhish.sHtML

[S55] C++：结构化绑定
来源：http://read.share.hesvh.cn/Article/details/gylohivvd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gnlqxdxhh.sHtML

[S56] C++：optional
来源：http://baike.zdbjq.cn/Article/details/ggnjakfrj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.zdbjq.cn/Article/details/geedpvlqq.sHtML

[S57] C++：编译期常量
来源：http://read.share.hesvh.cn/Article/details/geognzzch.sHtML

constexpr int N = 10;
来源：http://www.share.fehbvm.com/Article/details/ghuzgepwp.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fehbvm.com/Article/details/gsrfmsdlg.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.hesvh.cn/Article/details/gaigtodpc.sHtML

[S59] C++：静态断言
来源：http://mobile.zdbjq.cn/Article/details/gkasdcile.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.zdbjq.cn/Article/details/gotfuwbzp.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.zdbjq.cn/Article/details/gfpsossnn.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fehbvm.com/Article/details/gbpvdhiiv.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gbwsfuxbb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.zdbjq.cn/Article/details/gngulnmih.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gilinckvh.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fehbvm.com/Article/details/gducpsfbj.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/gkmmbzvzy.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.zdbjq.cn/Article/details/ghfuovajm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fehbvm.com/Article/details/gkitgownl.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.hesvh.cn/Article/details/gyxocxtjl.sHtML

"值: $b"
来源：http://baike.zdbjq.cn/Article/details/ghsvcxfem.sHtML

[T04] Kotlin：空安全
来源：http://3g.zdbjq.cn/Article/details/gwyjdtvkr.sHtML

val n: String? = null;  n?.length
来源：http://baike.hesvh.cn/Article/details/gzrgwmvgu.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.zdbjq.cn/Article/details/gastpobvh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.hesvh.cn/Article/details/gypvgvizl.sHtML

[T06] Kotlin：集合映射
来源：http://baike.hesvh.cn/Article/details/gkogghanw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.hesvh.cn/Article/details/gcxieklpg.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fehbvm.com/Article/details/gwjzvimkb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.hesvh.cn/Article/details/gcbkxvtgz.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.zdbjq.cn/Article/details/gtekandvc.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.zdbjq.cn/Article/details/gysfnqcbf.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fehbvm.com/Article/details/gnrhnkdxe.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.zdbjq.cn/Article/details/gvaagonrq.sHtML

[T10] Kotlin：默认参数
来源：http://3g.hesvh.cn/Article/details/gjldbnwcd.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.hesvh.cn/Article/details/grfdcncct.sHtML

[T11] Kotlin：协程
来源：http://mobile.zdbjq.cn/Article/details/ggbpflodr.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.zdbjq.cn/Article/details/gptkkzxdy.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.hesvh.cn/Article/details/gqdxaunwy.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.zdbjq.cn/Article/details/ghqzeclfd.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fehbvm.com/Article/details/gliuycuqf.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.hesvh.cn/Article/details/gniusjzra.sHtML

[T14] Kotlin：循环
来源：http://3g.hesvh.cn/Article/details/gnmiwjhtc.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/gfuufetew.sHtML

[T15] Kotlin：接口
来源：http://wap.zdbjq.cn/Article/details/gcmxpqijt.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.hesvh.cn/Article/details/gjvaziync.sHtML

[T16] Swift：Hello World
来源：http://blog.fehbvm.com/Article/details/gkjiqtoip.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gnuevadlg.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.zdbjq.cn/Article/details/gntwomlqv.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.hesvh.cn/Article/details/gbxbrzres.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gggxqgdnm.sHtML

"值: \(b)"
来源：http://read.share.fehbvm.com/Article/details/gixddubva.sHtML

[T19] Swift：可选绑定
来源：http://wap.fehbvm.com/Article/details/gbuygmsdf.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.zdbjq.cn/Article/details/goobwjwnn.sHtML

[T20] Swift：数组操作
来源：http://m.share.hesvh.cn/Article/details/gvxxlziqp.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.hesvh.cn/Article/details/gkacjjjxv.sHtML

[T21] Swift：遍历
来源：http://mobile.hesvh.cn/Article/details/gvoljnzdr.sHtML

for x in a { print(x) }
来源：http://3g.fehbvm.com/Article/details/gujwpuecu.sHtML

[T22] Swift：字典
来源：http://m.share.fehbvm.com/Article/details/ggnntulpj.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.zdbjq.cn/Article/details/gxcuuaych.sHtML

[T23] Swift：函数
来源：http://wap.zdbjq.cn/Article/details/glgqebzpu.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fehbvm.com/Article/details/ggjicoczm.sHtML

[T24] Swift：闭包
来源：http://m.share.zdbjq.cn/Article/details/gubditivx.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fehbvm.com/Article/details/gdpscrjjs.sHtML

[T25] Swift：结构体
来源：http://read.share.hesvh.cn/Article/details/gxrykycju.sHtML

struct P { var x: Int }
来源：http://wap.hesvh.cn/Article/details/goqrrjblr.sHtML

[T26] Swift：类与重写
来源：http://baike.zdbjq.cn/Article/details/gkaagsatl.sHtML

class A: Base { override func f() {} }
来源：http://www.share.hesvh.cn/Article/details/ggunhongr.sHtML

[T27] Swift：错误处理
来源：http://baike.zdbjq.cn/Article/details/gccmdidlw.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.hesvh.cn/Article/details/groptxswg.sHtML

[T28] Swift：枚举
来源：http://www.share.fehbvm.com/Article/details/gvjqquaxb.sHtML

enum Color { case red, green }
来源：http://read.share.zdbjq.cn/Article/details/gflobkfmp.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fehbvm.com/Article/details/gbaffismr.sHtML

guard let x = opt else { return }
来源：http://mobile.zdbjq.cn/Article/details/geruoxqjv.sHtML

[T30] Swift：协议
来源：http://wap.zdbjq.cn/Article/details/gfajxigqv.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.hesvh.cn/Article/details/gzlcwyzxk.sHtML

[T31] Lua：Hello World
来源：http://blog.zdbjq.cn/Article/details/gaqmlbdpp.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/gjgoubsvs.sHtML

[T32] Lua：局部变量
来源：http://3g.zdbjq.cn/Article/details/gkenvtfnt.sHtML

local a = 1
来源：http://3g.fehbvm.com/Article/details/gixrdegjc.sHtML

[T33] Lua：表（数组）
来源：http://3g.fehbvm.com/Article/details/gpptbggcm.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.fehbvm.com/Article/details/gurajqhsr.sHtML

[T34] Lua：遍历表
来源：http://blog.fehbvm.com/Article/details/gdvieoezv.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.zdbjq.cn/Article/details/glhfhfego.sHtML


<!-- 参考信息 -->