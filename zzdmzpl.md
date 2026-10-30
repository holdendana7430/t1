代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://www.blog.fehbvm.com/Article/details/guwvwfvff.sHtML

[R32] 参数个数校验
来源：http://m.share.fehbvm.com/Article/details/gygswriqx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/gbhmhawos.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.hesvh.cn/Article/details/glovhhbds.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.hesvh.cn/Article/details/gyxtshrdq.sHtML

[R34] 退出时清理
来源：http://read.share.hesvh.cn/Article/details/gjxuoremt.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/gnplewziy.sHtML

[R35] 后台执行并等待
来源：http://www.blog.zdbjq.cn/Article/details/gxolmhmcj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.hesvh.cn/Article/details/guurmunio.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fehbvm.com/Article/details/gazrrohva.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fehbvm.com/Article/details/gpqdsqmqz.sHtML

[R37] 把输出赋给变量
来源：http://wap.zdbjq.cn/Article/details/gswtbsmxq.sHtML

files=$(ls -1)
来源：http://blog.zdbjq.cn/Article/details/gnoysmqao.sHtML

[R38] 管道串联
来源：http://www.share.hesvh.cn/Article/details/gpafbzgfl.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.zdbjq.cn/Article/details/gqkkulslj.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.zdbjq.cn/Article/details/giamcxlml.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/gienzglfs.sHtML

[R40] 追加写日志
来源：http://www.m.share.zdbjq.cn/Article/details/gveautaah.sHtML

echo "log" >> out.log
来源：http://blog.fehbvm.com/Article/details/gruduedqi.sHtML

[R41] 丢弃输出
来源：http://m.share.hesvh.cn/Article/details/grmofochw.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.hesvh.cn/Article/details/gxzuvsqrm.sHtML

[R42] 输入重定向
来源：http://www.share.zdbjq.cn/Article/details/gqbkgzuav.sHtML

wc -l < a.txt
来源：http://mobile.hesvh.cn/Article/details/gvihujykp.sHtML

[R43] 按名字查找文件
来源：http://wap.fehbvm.com/Article/details/gglittczl.sHtML

find . -name "*.log" -type f
来源：http://www.blog.hesvh.cn/Article/details/ggtepqnnn.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.zdbjq.cn/Article/details/gcprtsfqw.sHtML

find . -mtime -7 -type f
来源：http://m.share.zdbjq.cn/Article/details/gkgeqgupj.sHtML

[R45] 批量删除
来源：http://m.share.fehbvm.com/Article/details/gqjwicmnu.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fehbvm.com/Article/details/gumjetxwl.sHtML

[R46] 递归替换文件内容
来源：http://www.share.zdbjq.cn/Article/details/gtumxeyyl.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.zdbjq.cn/Article/details/gdljzfbnh.sHtML

[R47] sed 单行替换
来源：http://baike.fehbvm.com/Article/details/gkkixxusq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gohdrrchf.sHtML

[R48] awk 取指定列
来源：http://baike.fehbvm.com/Article/details/ggyvuvzqf.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gqnbybmen.sHtML

[R49] awk 带条件
来源：http://www.share.hesvh.cn/Article/details/gkkmckome.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.hesvh.cn/Article/details/glwnqoabo.sHtML

[R50] awk 求和
来源：http://m.share.fehbvm.com/Article/details/gwruoogwl.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fehbvm.com/Article/details/gghfzqbqn.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.zdbjq.cn/Article/details/gqvymqvzf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fehbvm.com/Article/details/gxukdvehp.sHtML

[R52] 统计行数
来源：http://baike.fehbvm.com/Article/details/gbhxqideh.sHtML

wc -l a.txt
来源：http://mobile.zdbjq.cn/Article/details/grnhpdnzx.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fehbvm.com/Article/details/goodugrzz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.hesvh.cn/Article/details/gktocohoj.sHtML

[R54] 比较两个文件
来源：http://read.share.zdbjq.cn/Article/details/gvrrvhzmz.sHtML

diff a.txt b.txt
来源：http://3g.hesvh.cn/Article/details/gxrjilybb.sHtML

[R55] 压缩与解压
来源：http://blog.hesvh.cn/Article/details/gnxyjtnzd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.hesvh.cn/Article/details/gjxzrwtuj.sHtML

[R56] 远程拷贝
来源：http://www.share.zdbjq.cn/Article/details/gfhqiyihy.sHtML

scp file user@host:/path/
来源：http://read.share.zdbjq.cn/Article/details/gymihfyve.sHtML

[R57] 远程执行命令
来源：http://m.share.zdbjq.cn/Article/details/gzilymngd.sHtML

ssh user@host 'uptime'
来源：http://blog.hesvh.cn/Article/details/gpkmfbhls.sHtML

[R58] 下载文件
来源：http://www.share.fehbvm.com/Article/details/gwjedhmuy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fehbvm.com/Article/details/gwcdtxxbw.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gpkueoiyv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.hesvh.cn/Article/details/ggeelzzhc.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/gfrmmhcub.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fehbvm.com/Article/details/gnzcneqov.sHtML

[R61] 磁盘占用
来源：http://www.blog.zdbjq.cn/Article/details/ggyunqgfi.sHtML

df -h;  du -sh *
来源：http://blog.fehbvm.com/Article/details/gwenscjyu.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fehbvm.com/Article/details/gmpaixdyu.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.zdbjq.cn/Article/details/gvnyxsink.sHtML

[R63] 内存与进程
来源：http://baike.hesvh.cn/Article/details/gavhpkjad.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.zdbjq.cn/Article/details/gadaoweav.sHtML

[R64] 结束进程
来源：http://www.share.zdbjq.cn/Article/details/gpsnypcgy.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.hesvh.cn/Article/details/gqjxpnzmj.sHtML

[R65] 查看端口占用
来源：http://read.share.zdbjq.cn/Article/details/gcspprjdz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.zdbjq.cn/Article/details/goswcfemg.sHtML

[R66] 定时任务
来源：http://read.share.hesvh.cn/Article/details/gqmphkbkg.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fehbvm.com/Article/details/gxwziqhyz.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.hesvh.cn/Article/details/grymicmgo.sHtML

openssl rand -hex 16
来源：http://mobile.hesvh.cn/Article/details/gllsqhouu.sHtML

[R68] 计算文件校验值
来源：http://m.share.fehbvm.com/Article/details/gtnpnmxte.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.zdbjq.cn/Article/details/gasetzwpf.sHtML

[R69] 生成随机密码
来源：http://3g.hesvh.cn/Article/details/gvmnhphlr.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.zdbjq.cn/Article/details/gelxbuuof.sHtML

[R70] 时间戳与互转
来源：http://baike.hesvh.cn/Article/details/gabguswvd.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fehbvm.com/Article/details/ggzryeqxw.sHtML

[R71] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/gdzykteoc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fehbvm.com/Article/details/guiwptuks.sHtML

[R72] 等待端口就绪
来源：http://baike.fehbvm.com/Article/details/givukrqyf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/gmvsmntja.sHtML

[R73] 分割大日志
来源：http://www.share.zdbjq.cn/Article/details/gppqrwnzc.sHtML

split -l 1000 big.log part_
来源：http://3g.zdbjq.cn/Article/details/gexdmrfoq.sHtML

[R74] 批量重命名
来源：http://wap.zdbjq.cn/Article/details/gspcugzti.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.zdbjq.cn/Article/details/gjhvptvgl.sHtML

[R75] 导出环境变量
来源：http://wap.zdbjq.cn/Article/details/gsnttksok.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fehbvm.com/Article/details/gvhmfrlgk.sHtML

[R76] 使用临时文件
来源：http://3g.zdbjq.cn/Article/details/gkynlcsfm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/gzjsbtagy.sHtML

[R77] 读取用户输入
来源：http://www.share.zdbjq.cn/Article/details/gmyzdxapx.sHtML

read -rp "请输入: " ans
来源：http://m.share.hesvh.cn/Article/details/gmmmkeich.sHtML

[R78] 交互式菜单
来源：http://www.blog.fehbvm.com/Article/details/ghqdorodp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fehbvm.com/Article/details/gkkrwnybr.sHtML

[R79] 解析命令行选项
来源：http://www.share.fehbvm.com/Article/details/gmhgiysgc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.hesvh.cn/Article/details/gmstpflew.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fehbvm.com/Article/details/gnnzxzqfb.sHtML

time ./run.sh
来源：http://baike.zdbjq.cn/Article/details/gopshbmgw.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/grgeaqwfs.sHtML

S. C / C++ 专题
来源：http://read.share.zdbjq.cn/Article/details/gbppgrity.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gbrvngwnn.sHtML

[S01] C：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gxvkaicwi.sHtML

#include <stdio.h>
来源：http://www.blog.zdbjq.cn/Article/details/gatczixhf.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.hesvh.cn/Article/details/gekecpcou.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fehbvm.com/Article/details/gxiydeckd.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.zdbjq.cn/Article/details/gljzvlths.sHtML

[S03] C：读入整数
来源：http://wap.fehbvm.com/Article/details/gptvvkmbv.sHtML

int x; scanf("%d", &x);
来源：http://www.share.zdbjq.cn/Article/details/ghzanrlkb.sHtML

[S04] C：字符串复制
来源：http://www.blog.fehbvm.com/Article/details/gbclwnvpu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fehbvm.com/Article/details/gktkjwciz.sHtML

[S05] C：字符串长度
来源：http://read.share.hesvh.cn/Article/details/gguldgizz.sHtML

strlen(s)
来源：http://m.share.hesvh.cn/Article/details/gocjjochi.sHtML

[S06] C：字符串比较
来源：http://blog.zdbjq.cn/Article/details/gvymegzfq.sHtML

strcmp(a, b) == 0
来源：http://www.share.zdbjq.cn/Article/details/geouicbbw.sHtML

[S07] C：数组遍历求和
来源：http://baike.zdbjq.cn/Article/details/gcnuquhug.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.hesvh.cn/Article/details/gftrukdxl.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.hesvh.cn/Article/details/gfhhovxll.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.zdbjq.cn/Article/details/glzukvugb.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fehbvm.com/Article/details/govjejtyu.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.zdbjq.cn/Article/details/gjwethelt.sHtML

[S10] C：指针与解引用
来源：http://www.share.zdbjq.cn/Article/details/gmomqpxvl.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fehbvm.com/Article/details/gjjjcniqq.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gwkntrhsf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fehbvm.com/Article/details/gkxgqdgqe.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fehbvm.com/Article/details/gwhvzexyw.sHtML

fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/glcrtgelu.sHtML

[S12] C：写文件
来源：http://baike.fehbvm.com/Article/details/gsznmnlwz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gfssfhoru.sHtML

[S13] C：宏定义
来源：http://www.share.zdbjq.cn/Article/details/gostibfcz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.hesvh.cn/Article/details/geolgipls.sHtML

[S14] C：枚举
来源：http://baike.fehbvm.com/Article/details/gbyseynav.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.hesvh.cn/Article/details/gmavevjbd.sHtML

[S15] C：类型转换
来源：http://wap.hesvh.cn/Article/details/gcectauff.sHtML

(double) a / b
来源：http://read.share.hesvh.cn/Article/details/golximmhy.sHtML

[S16] C：位操作置位
来源：http://www.m.share.hesvh.cn/Article/details/glaoiicqu.sHtML

x |= (1 << 3);
来源：http://3g.hesvh.cn/Article/details/gldzpnfeo.sHtML

[S17] C：安全拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gwyhwbacg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.hesvh.cn/Article/details/graaojngs.sHtML

[S18] C：命令行参数
来源：http://www.blog.hesvh.cn/Article/details/geczhoivc.sHtML

int main(int argc, char **argv)
来源：http://read.share.hesvh.cn/Article/details/gjkxcrohy.sHtML

[S19] C：快速排序
来源：http://wap.zdbjq.cn/Article/details/gmzywjrav.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gvaewctde.sHtML

[S20] C：二分查找
来源：http://mobile.zdbjq.cn/Article/details/gibavywsr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/gnaftfdpd.sHtML

[S21] C：字符类别判断
来源：http://read.share.hesvh.cn/Article/details/gwgsirozl.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.hesvh.cn/Article/details/ggubeyukv.sHtML

[S22] C：字符串转数字
来源：http://mobile.hesvh.cn/Article/details/gkceapzlr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.hesvh.cn/Article/details/gtmstiukn.sHtML

[S23] C：随机数
来源：http://mobile.fehbvm.com/Article/details/gxluebdle.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.zdbjq.cn/Article/details/gyrmtpglv.sHtML

[S24] C：获取本地时间
来源：http://blog.hesvh.cn/Article/details/gbfrvtfgv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fehbvm.com/Article/details/gukezgmuu.sHtML

[S25] C：内存拷贝
来源：http://m.share.hesvh.cn/Article/details/gzasavgji.sHtML

memcpy(dst, src, n);
来源：http://blog.hesvh.cn/Article/details/gxwxqzysa.sHtML

[S26] C：内存清零
来源：http://3g.fehbvm.com/Article/details/glevvzdre.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fehbvm.com/Article/details/gwpswsekm.sHtML

[S27] C：定义常量
来源：http://m.share.hesvh.cn/Article/details/gaikzfzjm.sHtML

const double PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gqcfenqge.sHtML

[S28] C：静态变量
来源：http://baike.hesvh.cn/Article/details/gikfyxzbb.sHtML

static int counter = 0;
来源：http://m.share.zdbjq.cn/Article/details/glvndfqmh.sHtML

[S29] C：变参函数
来源：http://baike.fehbvm.com/Article/details/ghbwyhwqh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fehbvm.com/Article/details/gsznhkzal.sHtML

[S30] C：头文件保护
来源：http://baike.fehbvm.com/Article/details/gukzvnrso.sHtML

#ifndef X_H
来源：http://baike.zdbjq.cn/Article/details/gyqwqfwye.sHtML

#define X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gchheooni.sHtML

#endif
来源：http://wap.hesvh.cn/Article/details/gqdhhktik.sHtML

[S31] C++：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gwokyltrl.sHtML

#include <iostream>
来源：http://read.share.zdbjq.cn/Article/details/gnfvihldi.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fehbvm.com/Article/details/gzscmmtos.sHtML

[S32] C++：字符串
来源：http://read.share.hesvh.cn/Article/details/gfkcfhdgm.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.zdbjq.cn/Article/details/gyoxgdtjt.sHtML

[S33] C++：vector 增删
来源：http://mobile.hesvh.cn/Article/details/gzucahltu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.hesvh.cn/Article/details/gvkrwgnwb.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.hesvh.cn/Article/details/guheeiixo.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.hesvh.cn/Article/details/gmovemlox.sHtML

[S35] C++：map
来源：http://blog.zdbjq.cn/Article/details/gubkolccy.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/gliutxgtb.sHtML

[S36] C++：unordered_map
来源：http://wap.zdbjq.cn/Article/details/grayjycal.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gyonzmmdv.sHtML

[S37] C++：set
来源：http://read.share.fehbvm.com/Article/details/gihwtldid.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fehbvm.com/Article/details/gewnbjefx.sHtML

[S38] C++：排序
来源：http://mobile.fehbvm.com/Article/details/gxsbqouea.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.zdbjq.cn/Article/details/gonvzzpxp.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.hesvh.cn/Article/details/gwgczswhl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.hesvh.cn/Article/details/gzrqotnxa.sHtML

[S40] C++：查找元素
来源：http://m.share.fehbvm.com/Article/details/guaqctxou.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fehbvm.com/Article/details/gwbrrchrc.sHtML

[S41] C++：类与构造函数
来源：http://www.share.zdbjq.cn/Article/details/gtnawaimi.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.zdbjq.cn/Article/details/gsssolbya.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.hesvh.cn/Article/details/gwjfhptub.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.hesvh.cn/Article/details/gutyztamq.sHtML

[S43] C++：智能指针
来源：http://baike.zdbjq.cn/Article/details/gpvikuvvu.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.zdbjq.cn/Article/details/grucetlga.sHtML

[S44] C++：引用传参
来源：http://m.share.zdbjq.cn/Article/details/gufarbxqy.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.hesvh.cn/Article/details/glcptntwo.sHtML

[S45] C++：lambda
来源：http://3g.zdbjq.cn/Article/details/gwlghuwgk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.zdbjq.cn/Article/details/gwmzbxuqh.sHtML

[S46] C++：函数模板
来源：http://m.share.zdbjq.cn/Article/details/gmgcqobvv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.zdbjq.cn/Article/details/grsbfoyym.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.zdbjq.cn/Article/details/gektgwtwk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.hesvh.cn/Article/details/ggwmvptba.sHtML

[S48] C++：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gvybimrhw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.zdbjq.cn/Article/details/gbigtsklq.sHtML

while (std::getline(in, line)) { }
来源：http://blog.zdbjq.cn/Article/details/gaevjdwks.sHtML

[S49] C++：写文件
来源：http://blog.fehbvm.com/Article/details/garijicmh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fehbvm.com/Article/details/gyzlhyvee.sHtML

[S50] C++：格式化数字
来源：http://wap.zdbjq.cn/Article/details/gznicsbri.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.hesvh.cn/Article/details/ghxcnarpw.sHtML

[S51] C++：显式类型转换
来源：http://www.share.zdbjq.cn/Article/details/gjjuakbog.sHtML

static_cast<double>(a) / b
来源：http://blog.fehbvm.com/Article/details/guxjvkhlg.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fehbvm.com/Article/details/gskfjxxrx.sHtML

int size() const noexcept { return n_; }
来源：http://wap.hesvh.cn/Article/details/goubtzsbb.sHtML

[S53] C++：移动语义
来源：http://mobile.hesvh.cn/Article/details/gzifrrzmq.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.zdbjq.cn/Article/details/gwfyxebfe.sHtML

[S54] C++：异常处理
来源：http://www.blog.zdbjq.cn/Article/details/glbptqsvo.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.hesvh.cn/Article/details/gkaxytdve.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fehbvm.com/Article/details/gftterrgq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.hesvh.cn/Article/details/gqtzmlquv.sHtML

[S56] C++：optional
来源：http://www.m.share.zdbjq.cn/Article/details/gbowcaoky.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.hesvh.cn/Article/details/ggkjzxhyq.sHtML

[S57] C++：编译期常量
来源：http://3g.zdbjq.cn/Article/details/gmenvbpzo.sHtML

constexpr int N = 10;
来源：http://m.share.zdbjq.cn/Article/details/gqemwuiif.sHtML

[S58] C++：命名空间
来源：http://blog.hesvh.cn/Article/details/gpuazgmfl.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.hesvh.cn/Article/details/gyhzrsrvj.sHtML

[S59] C++：静态断言
来源：http://mobile.hesvh.cn/Article/details/gjeuvpvno.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.zdbjq.cn/Article/details/gsashqukv.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fehbvm.com/Article/details/gunscywft.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fehbvm.com/Article/details/giubxiakx.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ghroxusbc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fehbvm.com/Article/details/gcokdcrip.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gjhepztqj.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fehbvm.com/Article/details/gnygreonj.sHtML

println("Hello")
来源：http://read.share.zdbjq.cn/Article/details/galluphpl.sHtML

[T02] Kotlin：变量
来源：http://www.blog.zdbjq.cn/Article/details/geyhevrpa.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.zdbjq.cn/Article/details/gyctbdedk.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fehbvm.com/Article/details/gkzzbwxjp.sHtML

"值: $b"
来源：http://read.share.zdbjq.cn/Article/details/gzukqnbnr.sHtML

[T04] Kotlin：空安全
来源：http://www.share.hesvh.cn/Article/details/gmsnrvnjg.sHtML

val n: String? = null;  n?.length
来源：http://wap.fehbvm.com/Article/details/gjjoabdyu.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.hesvh.cn/Article/details/gykypxskd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.zdbjq.cn/Article/details/gomenqhmv.sHtML

[T06] Kotlin：集合映射
来源：http://3g.hesvh.cn/Article/details/gyuiytrau.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fehbvm.com/Article/details/ghdqzxwsz.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fehbvm.com/Article/details/gtyaizbna.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.hesvh.cn/Article/details/gewrjkrzj.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fehbvm.com/Article/details/gcailvzcu.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fehbvm.com/Article/details/gynljhkeg.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.zdbjq.cn/Article/details/gcghvpioq.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fehbvm.com/Article/details/gfwtpmzff.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fehbvm.com/Article/details/gciocswhd.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fehbvm.com/Article/details/gamqyttrt.sHtML

[T11] Kotlin：协程
来源：http://read.share.hesvh.cn/Article/details/gsrsffvli.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fehbvm.com/Article/details/gbdatjnwh.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fehbvm.com/Article/details/gjsogianl.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gfjgivgbo.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.hesvh.cn/Article/details/gaewjxsyk.sHtML

val m = mapOf("a" to 1)
来源：http://blog.zdbjq.cn/Article/details/gfvoiqlmv.sHtML

[T14] Kotlin：循环
来源：http://3g.hesvh.cn/Article/details/gusyhcggo.sHtML

for (i in 1..10) println(i)
来源：http://read.share.hesvh.cn/Article/details/gfjyyrxyx.sHtML

[T15] Kotlin：接口
来源：http://mobile.fehbvm.com/Article/details/gwbwwhhfa.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.zdbjq.cn/Article/details/ggkateqcx.sHtML

[T16] Swift：Hello World
来源：http://m.share.fehbvm.com/Article/details/gpeipebia.sHtML

print("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gtncpgcmo.sHtML

[T17] Swift：变量与常量
来源：http://blog.hesvh.cn/Article/details/gmnvlcurt.sHtML

var a = 1;  let b = 2
来源：http://m.share.zdbjq.cn/Article/details/guktfglzq.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gyvfewvwh.sHtML

"值: \(b)"
来源：http://3g.hesvh.cn/Article/details/gqtxalgmu.sHtML

[T19] Swift：可选绑定
来源：http://3g.fehbvm.com/Article/details/gxvvpcyic.sHtML

if let n = opt { print(n) }
来源：http://www.blog.hesvh.cn/Article/details/ghmhrrcxs.sHtML

[T20] Swift：数组操作
来源：http://baike.hesvh.cn/Article/details/gbdlmpoej.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.hesvh.cn/Article/details/ghuubjmgv.sHtML

[T21] Swift：遍历
来源：http://read.share.zdbjq.cn/Article/details/gkxmslogs.sHtML

for x in a { print(x) }
来源：http://blog.hesvh.cn/Article/details/gnxclkhea.sHtML

[T22] Swift：字典
来源：http://www.m.share.hesvh.cn/Article/details/gnyxvuwsc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.hesvh.cn/Article/details/gifhszgsh.sHtML

[T23] Swift：函数
来源：http://baike.hesvh.cn/Article/details/gaipglvfb.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.zdbjq.cn/Article/details/gyychyqro.sHtML

[T24] Swift：闭包
来源：http://www.share.fehbvm.com/Article/details/gaxrkzvwe.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fehbvm.com/Article/details/gtsgdckqs.sHtML

[T25] Swift：结构体
来源：http://www.blog.hesvh.cn/Article/details/gtdkcnczr.sHtML

struct P { var x: Int }
来源：http://3g.hesvh.cn/Article/details/gxfmxakvl.sHtML

[T26] Swift：类与重写
来源：http://baike.hesvh.cn/Article/details/ghnsuxiee.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.zdbjq.cn/Article/details/gxnryriwh.sHtML

[T27] Swift：错误处理
来源：http://wap.fehbvm.com/Article/details/geucwqpmg.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fehbvm.com/Article/details/gvppxmick.sHtML

[T28] Swift：枚举
来源：http://blog.hesvh.cn/Article/details/gvmczzrth.sHtML

enum Color { case red, green }
来源：http://blog.hesvh.cn/Article/details/glgxqlnib.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.zdbjq.cn/Article/details/gyypvfpax.sHtML

guard let x = opt else { return }
来源：http://blog.fehbvm.com/Article/details/gsggbxihm.sHtML

[T30] Swift：协议
来源：http://3g.fehbvm.com/Article/details/gmyzcetbd.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fehbvm.com/Article/details/gkdmiylgr.sHtML

[T31] Lua：Hello World
来源：http://3g.zdbjq.cn/Article/details/gmxamvwjw.sHtML

print("Hello")
来源：http://mobile.hesvh.cn/Article/details/gexsohjpr.sHtML

[T32] Lua：局部变量
来源：http://baike.zdbjq.cn/Article/details/gtcoizkza.sHtML

local a = 1
来源：http://www.share.zdbjq.cn/Article/details/gkvdouilu.sHtML

[T33] Lua：表（数组）
来源：http://baike.zdbjq.cn/Article/details/gsxwyvjna.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fehbvm.com/Article/details/grvuwyzcn.sHtML

[T34] Lua：遍历表
来源：http://baike.zdbjq.cn/Article/details/gzrtdwglq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.hesvh.cn/Article/details/glztvbbsf.sHtML


<!-- 参考信息 -->