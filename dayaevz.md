代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://wap.zdbjq.cn/Article/details/gqpdznyaa.sHtML

[R32] 参数个数校验
来源：http://wap.fehbvm.com/Article/details/gmirsbdrd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/gxlofkzfu.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.zdbjq.cn/Article/details/gdrbhtdej.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.zdbjq.cn/Article/details/gytogkywq.sHtML

[R34] 退出时清理
来源：http://blog.zdbjq.cn/Article/details/gmqojmphl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/gjrxeinbr.sHtML

[R35] 后台执行并等待
来源：http://baike.hesvh.cn/Article/details/glrncmeio.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fehbvm.com/Article/details/ghqorarvy.sHtML

[R36] 并发执行多个任务
来源：http://www.share.hesvh.cn/Article/details/gzzmcsjvx.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.zdbjq.cn/Article/details/gnjafnxmg.sHtML

[R37] 把输出赋给变量
来源：http://blog.zdbjq.cn/Article/details/gltwadsuj.sHtML

files=$(ls -1)
来源：http://www.blog.hesvh.cn/Article/details/gcpyecdxl.sHtML

[R38] 管道串联
来源：http://www.m.share.zdbjq.cn/Article/details/gbvkaaerr.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.hesvh.cn/Article/details/gweccqrtg.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.hesvh.cn/Article/details/gcqmzenks.sHtML

cmd > out.log 2>&1
来源：http://wap.zdbjq.cn/Article/details/gzjjtpdnr.sHtML

[R40] 追加写日志
来源：http://blog.fehbvm.com/Article/details/gyomtgorm.sHtML

echo "log" >> out.log
来源：http://www.blog.fehbvm.com/Article/details/godhvvcrb.sHtML

[R41] 丢弃输出
来源：http://read.share.zdbjq.cn/Article/details/getpuzkpt.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fehbvm.com/Article/details/gzrtvwcbe.sHtML

[R42] 输入重定向
来源：http://www.share.zdbjq.cn/Article/details/gaqdliscs.sHtML

wc -l < a.txt
来源：http://blog.zdbjq.cn/Article/details/gboyxvrvx.sHtML

[R43] 按名字查找文件
来源：http://3g.hesvh.cn/Article/details/glwdjwocz.sHtML

find . -name "*.log" -type f
来源：http://wap.fehbvm.com/Article/details/gjtrxxdqb.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.zdbjq.cn/Article/details/gwaeecvqs.sHtML

find . -mtime -7 -type f
来源：http://mobile.zdbjq.cn/Article/details/gotrirwpm.sHtML

[R45] 批量删除
来源：http://baike.hesvh.cn/Article/details/gqylklfqi.sHtML

find . -name "*.tmp" -delete
来源：http://blog.zdbjq.cn/Article/details/gtenwgpqe.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fehbvm.com/Article/details/gsnagrbim.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.zdbjq.cn/Article/details/gfhbxodnd.sHtML

[R47] sed 单行替换
来源：http://blog.zdbjq.cn/Article/details/glfnfvwei.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/guhudttxv.sHtML

[R48] awk 取指定列
来源：http://3g.zdbjq.cn/Article/details/gtihzzfph.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.hesvh.cn/Article/details/gneyzaqvh.sHtML

[R49] awk 带条件
来源：http://mobile.zdbjq.cn/Article/details/gwejenbal.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fehbvm.com/Article/details/grzdsztit.sHtML

[R50] awk 求和
来源：http://www.share.hesvh.cn/Article/details/gnzouejsr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/ggocwziol.sHtML

[R51] 排序去重取前几
来源：http://m.share.hesvh.cn/Article/details/gvwoxlkgl.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.zdbjq.cn/Article/details/glaydzedo.sHtML

[R52] 统计行数
来源：http://www.m.share.fehbvm.com/Article/details/gvwcvdsxa.sHtML

wc -l a.txt
来源：http://baike.zdbjq.cn/Article/details/gyjbcyvht.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.hesvh.cn/Article/details/gbfbbicfw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.hesvh.cn/Article/details/gzfzjlfje.sHtML

[R54] 比较两个文件
来源：http://m.share.hesvh.cn/Article/details/gqzdsrkuk.sHtML

diff a.txt b.txt
来源：http://read.share.hesvh.cn/Article/details/gzjukdfic.sHtML

[R55] 压缩与解压
来源：http://m.share.zdbjq.cn/Article/details/gqzigezky.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fehbvm.com/Article/details/gqvdnfhcy.sHtML

[R56] 远程拷贝
来源：http://blog.zdbjq.cn/Article/details/gtsqqttmt.sHtML

scp file user@host:/path/
来源：http://baike.hesvh.cn/Article/details/gyutijxdx.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fehbvm.com/Article/details/gqojjhfhm.sHtML

ssh user@host 'uptime'
来源：http://blog.zdbjq.cn/Article/details/guvuqueqo.sHtML

[R58] 下载文件
来源：http://wap.zdbjq.cn/Article/details/goggtpjft.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.hesvh.cn/Article/details/gqmkuatbs.sHtML

[R59] 发 POST JSON
来源：http://wap.zdbjq.cn/Article/details/ggbksyuge.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.zdbjq.cn/Article/details/ggqosjzpe.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/gffbmewzj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fehbvm.com/Article/details/gxsfjymbc.sHtML

[R61] 磁盘占用
来源：http://www.blog.fehbvm.com/Article/details/gnaotkskq.sHtML

df -h;  du -sh *
来源：http://www.blog.zdbjq.cn/Article/details/gepcjgmtn.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fehbvm.com/Article/details/gfbbfyiwg.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fehbvm.com/Article/details/geooietlq.sHtML

[R63] 内存与进程
来源：http://blog.hesvh.cn/Article/details/gxchzfvkv.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fehbvm.com/Article/details/gceigiwzo.sHtML

[R64] 结束进程
来源：http://m.share.zdbjq.cn/Article/details/gacxaxrkf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.zdbjq.cn/Article/details/gvnrdcbdk.sHtML

[R65] 查看端口占用
来源：http://blog.zdbjq.cn/Article/details/ghujmvsor.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.hesvh.cn/Article/details/gaqotwmsy.sHtML

[R66] 定时任务
来源：http://wap.fehbvm.com/Article/details/gktcksqaz.sHtML

crontab -e;  crontab -l
来源：http://blog.fehbvm.com/Article/details/gmlvzsxcp.sHtML

[R67] 生成随机十六进制串
来源：http://3g.zdbjq.cn/Article/details/gqcivaege.sHtML

openssl rand -hex 16
来源：http://read.share.zdbjq.cn/Article/details/gggbutvvn.sHtML

[R68] 计算文件校验值
来源：http://blog.zdbjq.cn/Article/details/glrmcnwzk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fehbvm.com/Article/details/gauimoxvi.sHtML

[R69] 生成随机密码
来源：http://www.blog.zdbjq.cn/Article/details/gpmrdnnzn.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fehbvm.com/Article/details/glfeykcui.sHtML

[R70] 时间戳与互转
来源：http://read.share.hesvh.cn/Article/details/gpwyzzbfk.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.zdbjq.cn/Article/details/gugljotxh.sHtML

[R71] 日期格式化
来源：http://wap.fehbvm.com/Article/details/gfmvvkijm.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fehbvm.com/Article/details/glgrvzpxn.sHtML

[R72] 等待端口就绪
来源：http://baike.zdbjq.cn/Article/details/gaadxnhvq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/gnjpogebz.sHtML

[R73] 分割大日志
来源：http://www.blog.hesvh.cn/Article/details/ggiicyxmn.sHtML

split -l 1000 big.log part_
来源：http://wap.fehbvm.com/Article/details/gjkwiyfjy.sHtML

[R74] 批量重命名
来源：http://baike.fehbvm.com/Article/details/gehczdphg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fehbvm.com/Article/details/gimfihsqq.sHtML

[R75] 导出环境变量
来源：http://read.share.hesvh.cn/Article/details/gazsrspno.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fehbvm.com/Article/details/gndcappdd.sHtML

[R76] 使用临时文件
来源：http://3g.zdbjq.cn/Article/details/gkkjoofiz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/gpxmnygjg.sHtML

[R77] 读取用户输入
来源：http://read.share.fehbvm.com/Article/details/gztnstteq.sHtML

read -rp "请输入: " ans
来源：http://m.share.zdbjq.cn/Article/details/gtbdgtphr.sHtML

[R78] 交互式菜单
来源：http://wap.zdbjq.cn/Article/details/gmmoptniq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fehbvm.com/Article/details/gbmrafdpx.sHtML

[R79] 解析命令行选项
来源：http://mobile.zdbjq.cn/Article/details/guuvuzzyb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.zdbjq.cn/Article/details/gftcjuecd.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.zdbjq.cn/Article/details/ggmpmnszs.sHtML

time ./run.sh
来源：http://m.share.hesvh.cn/Article/details/gwiudeisl.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gjfrvuvtj.sHtML

S. C / C++ 专题
来源：http://3g.fehbvm.com/Article/details/gwghcnjsa.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gkpwijism.sHtML

[S01] C：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/ghldxjsqj.sHtML

#include <stdio.h>
来源：http://www.m.share.zdbjq.cn/Article/details/gmeggiqcn.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.hesvh.cn/Article/details/gutsotipo.sHtML

[S02] C：变量与格式化输出
来源：http://wap.zdbjq.cn/Article/details/gzvctidmn.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.hesvh.cn/Article/details/ggtxrwpmx.sHtML

[S03] C：读入整数
来源：http://wap.zdbjq.cn/Article/details/ghywejpip.sHtML

int x; scanf("%d", &x);
来源：http://wap.fehbvm.com/Article/details/goplamtlw.sHtML

[S04] C：字符串复制
来源：http://www.share.hesvh.cn/Article/details/gtcmhxjga.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.zdbjq.cn/Article/details/gqrljujlb.sHtML

[S05] C：字符串长度
来源：http://blog.hesvh.cn/Article/details/ghhuktowv.sHtML

strlen(s)
来源：http://www.share.hesvh.cn/Article/details/gpjlavekj.sHtML

[S06] C：字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gilevngnj.sHtML

strcmp(a, b) == 0
来源：http://www.blog.zdbjq.cn/Article/details/gsohzrfik.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fehbvm.com/Article/details/ghqadqvkh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.zdbjq.cn/Article/details/gmjnksyiu.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.hesvh.cn/Article/details/ggicpcafm.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.hesvh.cn/Article/details/goupmmvbf.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fehbvm.com/Article/details/gzfumqkty.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.zdbjq.cn/Article/details/gnztethqw.sHtML

[S10] C：指针与解引用
来源：http://3g.zdbjq.cn/Article/details/guzbzuufu.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fehbvm.com/Article/details/ghwgvsfpz.sHtML

[S11] C：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gmlalvzfl.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.zdbjq.cn/Article/details/glrnvemev.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gatzihgdt.sHtML

fclose(f);
来源：http://3g.fehbvm.com/Article/details/gymlcafhl.sHtML

[S12] C：写文件
来源：http://wap.hesvh.cn/Article/details/glnmsqphv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.zdbjq.cn/Article/details/gepeltojy.sHtML

[S13] C：宏定义
来源：http://blog.hesvh.cn/Article/details/gichhmdvy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.hesvh.cn/Article/details/ggkqvlixu.sHtML

[S14] C：枚举
来源：http://baike.fehbvm.com/Article/details/gyctmhtjv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fehbvm.com/Article/details/godtukbmr.sHtML

[S15] C：类型转换
来源：http://mobile.zdbjq.cn/Article/details/gyijbihvq.sHtML

(double) a / b
来源：http://read.share.hesvh.cn/Article/details/gvumqvhoz.sHtML

[S16] C：位操作置位
来源：http://wap.hesvh.cn/Article/details/gttfklwgh.sHtML

x |= (1 << 3);
来源：http://wap.fehbvm.com/Article/details/gibuotttx.sHtML

[S17] C：安全拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gsotmjqqg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.zdbjq.cn/Article/details/gajcgpvtw.sHtML

[S18] C：命令行参数
来源：http://www.blog.fehbvm.com/Article/details/gcwxrikdo.sHtML

int main(int argc, char **argv)
来源：http://wap.zdbjq.cn/Article/details/gbiotnlhl.sHtML

[S19] C：快速排序
来源：http://www.blog.hesvh.cn/Article/details/gicsgyqlq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/geqgdecpz.sHtML

[S20] C：二分查找
来源：http://m.share.hesvh.cn/Article/details/ghqtfqvmb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/genrzvfhp.sHtML

[S21] C：字符类别判断
来源：http://mobile.fehbvm.com/Article/details/gfcrxfadk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.zdbjq.cn/Article/details/gsmdsgqee.sHtML

[S22] C：字符串转数字
来源：http://mobile.zdbjq.cn/Article/details/giuzbcidd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.hesvh.cn/Article/details/gqnvbcide.sHtML

[S23] C：随机数
来源：http://read.share.hesvh.cn/Article/details/gmzofpjid.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.hesvh.cn/Article/details/gonolwymg.sHtML

[S24] C：获取本地时间
来源：http://www.blog.zdbjq.cn/Article/details/ghcsgqzkt.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fehbvm.com/Article/details/gaefjnbty.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gwpgxhtgn.sHtML

memcpy(dst, src, n);
来源：http://wap.fehbvm.com/Article/details/gcjhsyxic.sHtML

[S26] C：内存清零
来源：http://blog.hesvh.cn/Article/details/gutmatgjy.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fehbvm.com/Article/details/gubwwgmru.sHtML

[S27] C：定义常量
来源：http://m.share.fehbvm.com/Article/details/gatldjpws.sHtML

const double PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gnktxudgv.sHtML

[S28] C：静态变量
来源：http://www.blog.hesvh.cn/Article/details/giagfoepj.sHtML

static int counter = 0;
来源：http://blog.fehbvm.com/Article/details/gvtqrxxvt.sHtML

[S29] C：变参函数
来源：http://read.share.hesvh.cn/Article/details/gsfikgfkx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.zdbjq.cn/Article/details/goaxmombc.sHtML

[S30] C：头文件保护
来源：http://blog.hesvh.cn/Article/details/gcnnnuuga.sHtML

#ifndef X_H
来源：http://3g.hesvh.cn/Article/details/gekxcfwna.sHtML

#define X_H
来源：http://blog.fehbvm.com/Article/details/goqbrdiyj.sHtML

#endif
来源：http://wap.hesvh.cn/Article/details/ggiyreyrk.sHtML

[S31] C++：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gwdjcuzmr.sHtML

#include <iostream>
来源：http://wap.zdbjq.cn/Article/details/gzvonjgpo.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fehbvm.com/Article/details/gghtpjmsr.sHtML

[S32] C++：字符串
来源：http://3g.hesvh.cn/Article/details/gobvqetxz.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.hesvh.cn/Article/details/gaohhvyft.sHtML

[S33] C++：vector 增删
来源：http://baike.fehbvm.com/Article/details/gjxzklisw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.zdbjq.cn/Article/details/grhuskmlk.sHtML

[S34] C++：遍历 vector
来源：http://wap.hesvh.cn/Article/details/gufaklshd.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.zdbjq.cn/Article/details/gryyuvdzd.sHtML

[S35] C++：map
来源：http://www.blog.zdbjq.cn/Article/details/ggsdbzgyd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/gxfujtrtj.sHtML

[S36] C++：unordered_map
来源：http://read.share.fehbvm.com/Article/details/ggtxqepsf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/gpdoadvkc.sHtML

[S37] C++：set
来源：http://www.m.share.fehbvm.com/Article/details/gtppepnlt.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.hesvh.cn/Article/details/gfhvbwquo.sHtML

[S38] C++：排序
来源：http://mobile.fehbvm.com/Article/details/gogxmyqbe.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.zdbjq.cn/Article/details/gtzecwssw.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.hesvh.cn/Article/details/gkmjmtozh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.hesvh.cn/Article/details/gkjtifwef.sHtML

[S40] C++：查找元素
来源：http://read.share.fehbvm.com/Article/details/gfbxstrud.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.hesvh.cn/Article/details/gzvbfgqxw.sHtML

[S41] C++：类与构造函数
来源：http://www.share.hesvh.cn/Article/details/gkvckrsqh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.zdbjq.cn/Article/details/gqxxnbpou.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fehbvm.com/Article/details/gcjoamhuv.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fehbvm.com/Article/details/gkuresjzg.sHtML

[S43] C++：智能指针
来源：http://blog.hesvh.cn/Article/details/gpfqcxgie.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.hesvh.cn/Article/details/geossanhm.sHtML

[S44] C++：引用传参
来源：http://mobile.hesvh.cn/Article/details/gpsdxvzzm.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.hesvh.cn/Article/details/gbjruynik.sHtML

[S45] C++：lambda
来源：http://www.m.share.zdbjq.cn/Article/details/ggotjvbhk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.zdbjq.cn/Article/details/ggvnjcxwy.sHtML

[S46] C++：函数模板
来源：http://www.blog.fehbvm.com/Article/details/gcqvazirz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.hesvh.cn/Article/details/gcnoyusaw.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fehbvm.com/Article/details/gfdrtkupe.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fehbvm.com/Article/details/gnmwailrl.sHtML

[S48] C++：逐行读文件
来源：http://baike.hesvh.cn/Article/details/guxuvjjbz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.hesvh.cn/Article/details/gesxvciri.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fehbvm.com/Article/details/gmvawwvpf.sHtML

[S49] C++：写文件
来源：http://read.share.fehbvm.com/Article/details/gkbpwzbap.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.hesvh.cn/Article/details/gnuheirxs.sHtML

[S50] C++：格式化数字
来源：http://3g.hesvh.cn/Article/details/glnoqemxq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gbpgyghpm.sHtML

[S51] C++：显式类型转换
来源：http://blog.zdbjq.cn/Article/details/gvnrucnup.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.zdbjq.cn/Article/details/gsybgukpk.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.hesvh.cn/Article/details/gjqznnfbz.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fehbvm.com/Article/details/gkiyukoqs.sHtML

[S53] C++：移动语义
来源：http://baike.fehbvm.com/Article/details/gnmcbiobs.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.hesvh.cn/Article/details/gkdmyjlsj.sHtML

[S54] C++：异常处理
来源：http://www.blog.hesvh.cn/Article/details/gittcuchb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.zdbjq.cn/Article/details/gijpmzknx.sHtML

[S55] C++：结构化绑定
来源：http://m.share.hesvh.cn/Article/details/grsccwony.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.hesvh.cn/Article/details/gusxxqkre.sHtML

[S56] C++：optional
来源：http://mobile.hesvh.cn/Article/details/gtiearbha.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.zdbjq.cn/Article/details/gzyvblyli.sHtML

[S57] C++：编译期常量
来源：http://blog.fehbvm.com/Article/details/gajbfnjit.sHtML

constexpr int N = 10;
来源：http://3g.fehbvm.com/Article/details/gztfvilvq.sHtML

[S58] C++：命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/gupkbgnnm.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.zdbjq.cn/Article/details/gcwpllajl.sHtML

[S59] C++：静态断言
来源：http://mobile.fehbvm.com/Article/details/gvirbrkpp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.zdbjq.cn/Article/details/gbiavhcuj.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.zdbjq.cn/Article/details/gbuqakiia.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.hesvh.cn/Article/details/gxjcysehw.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gktpdlahx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.hesvh.cn/Article/details/gqlndjpee.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gqmkjpqaf.sHtML

[T01] Kotlin：Hello World
来源：http://baike.zdbjq.cn/Article/details/gudcozuiy.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/gmcehkvzq.sHtML

[T02] Kotlin：变量
来源：http://wap.zdbjq.cn/Article/details/goerrfzhj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.zdbjq.cn/Article/details/gkqsjjkgh.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.hesvh.cn/Article/details/gsovzfasg.sHtML

"值: $b"
来源：http://wap.fehbvm.com/Article/details/gilsugoxr.sHtML

[T04] Kotlin：空安全
来源：http://blog.hesvh.cn/Article/details/goyrlklrk.sHtML

val n: String? = null;  n?.length
来源：http://blog.zdbjq.cn/Article/details/gyegpblkm.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fehbvm.com/Article/details/gomylvuql.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.zdbjq.cn/Article/details/gqoypupwq.sHtML

[T06] Kotlin：集合映射
来源：http://blog.zdbjq.cn/Article/details/gqokzrctm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fehbvm.com/Article/details/gsftgwwrk.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gssmppnvo.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fehbvm.com/Article/details/ghomzxxdi.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.zdbjq.cn/Article/details/gpaqnmaju.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.hesvh.cn/Article/details/ggojrpiyn.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fehbvm.com/Article/details/gciljzntm.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fehbvm.com/Article/details/ghyfqsrut.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.hesvh.cn/Article/details/gkvsqzzon.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fehbvm.com/Article/details/gvxftdjyq.sHtML

[T11] Kotlin：协程
来源：http://blog.zdbjq.cn/Article/details/giogitshn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.zdbjq.cn/Article/details/gmkqbuzcw.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.hesvh.cn/Article/details/gwecacpmz.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gucrnbbns.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fehbvm.com/Article/details/gzesutmee.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gimhntnxt.sHtML

[T14] Kotlin：循环
来源：http://blog.fehbvm.com/Article/details/gttgypirf.sHtML

for (i in 1..10) println(i)
来源：http://blog.zdbjq.cn/Article/details/gnciwnoev.sHtML

[T15] Kotlin：接口
来源：http://www.share.zdbjq.cn/Article/details/gkbrmvxqv.sHtML

interface Shape { fun area(): Double }
来源：http://baike.zdbjq.cn/Article/details/gyqwllixh.sHtML

[T16] Swift：Hello World
来源：http://www.share.fehbvm.com/Article/details/gxxwdbbta.sHtML

print("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gkkccywfd.sHtML

[T17] Swift：变量与常量
来源：http://m.share.zdbjq.cn/Article/details/gzmtqbhsr.sHtML

var a = 1;  let b = 2
来源：http://www.share.fehbvm.com/Article/details/gptxwjuev.sHtML

[T18] Swift：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gdspgmhvk.sHtML

"值: \(b)"
来源：http://blog.hesvh.cn/Article/details/gxypisjsi.sHtML

[T19] Swift：可选绑定
来源：http://wap.fehbvm.com/Article/details/geunfclim.sHtML

if let n = opt { print(n) }
来源：http://3g.hesvh.cn/Article/details/ggtlruhdn.sHtML

[T20] Swift：数组操作
来源：http://www.blog.hesvh.cn/Article/details/gemrxpjpp.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fehbvm.com/Article/details/guziaargu.sHtML

[T21] Swift：遍历
来源：http://blog.hesvh.cn/Article/details/gdjgxkpgg.sHtML

for x in a { print(x) }
来源：http://www.share.fehbvm.com/Article/details/gwivnzmns.sHtML

[T22] Swift：字典
来源：http://read.share.hesvh.cn/Article/details/ginilbqik.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.zdbjq.cn/Article/details/gsymxcffc.sHtML

[T23] Swift：函数
来源：http://mobile.zdbjq.cn/Article/details/guoezmcpn.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.zdbjq.cn/Article/details/gopnmpxeh.sHtML

[T24] Swift：闭包
来源：http://read.share.fehbvm.com/Article/details/gemhfppgi.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fehbvm.com/Article/details/gyqrfxtrm.sHtML

[T25] Swift：结构体
来源：http://m.share.zdbjq.cn/Article/details/gehtrqzpx.sHtML

struct P { var x: Int }
来源：http://mobile.zdbjq.cn/Article/details/gupzjhekn.sHtML

[T26] Swift：类与重写
来源：http://www.blog.zdbjq.cn/Article/details/gvjuphxzc.sHtML

class A: Base { override func f() {} }
来源：http://read.share.zdbjq.cn/Article/details/gwtiohwig.sHtML

[T27] Swift：错误处理
来源：http://3g.hesvh.cn/Article/details/gqhvdgkai.sHtML

do { try f() } catch { print(error) }
来源：http://baike.hesvh.cn/Article/details/ghpmrfszt.sHtML

[T28] Swift：枚举
来源：http://wap.zdbjq.cn/Article/details/gfavvupof.sHtML

enum Color { case red, green }
来源：http://mobile.zdbjq.cn/Article/details/gogsoxdwy.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.zdbjq.cn/Article/details/gbftufgna.sHtML

guard let x = opt else { return }
来源：http://www.share.zdbjq.cn/Article/details/gqcqpxbtk.sHtML

[T30] Swift：协议
来源：http://www.m.share.fehbvm.com/Article/details/gotzjfffh.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.hesvh.cn/Article/details/glgjslpkw.sHtML

[T31] Lua：Hello World
来源：http://wap.zdbjq.cn/Article/details/gaxnhddtq.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gmfwghggk.sHtML

[T32] Lua：局部变量
来源：http://wap.hesvh.cn/Article/details/gokollrmy.sHtML

local a = 1
来源：http://m.share.hesvh.cn/Article/details/gcgzexbjx.sHtML

[T33] Lua：表（数组）
来源：http://www.share.zdbjq.cn/Article/details/gteeczrpk.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.hesvh.cn/Article/details/gnrpfbcej.sHtML

[T34] Lua：遍历表
来源：http://wap.hesvh.cn/Article/details/gfqhjawso.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.hesvh.cn/Article/details/gxcfyejhm.sHtML


<!-- 参考信息 -->