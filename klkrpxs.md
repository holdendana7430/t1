代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.hesvh.cn/Article/details/gsrzrqphh.sHtML

[R34] 退出时清理
来源：http://baike.hesvh.cn/Article/details/ghfdonjav.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/gpsdhydwt.sHtML

[R35] 后台执行并等待
来源：http://baike.hesvh.cn/Article/details/gxrlwnbga.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.zdbjq.cn/Article/details/gyvqkgehv.sHtML

[R36] 并发执行多个任务
来源：http://wap.hesvh.cn/Article/details/gaaqkiibk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.zdbjq.cn/Article/details/gknrwinrs.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fehbvm.com/Article/details/gweyhqqto.sHtML

files=$(ls -1)
来源：http://wap.fehbvm.com/Article/details/gqnsckiae.sHtML

[R38] 管道串联
来源：http://3g.zdbjq.cn/Article/details/gbdpvaooq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fehbvm.com/Article/details/gykbjvcpk.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.hesvh.cn/Article/details/gdzxxjtcp.sHtML

cmd > out.log 2>&1
来源：http://read.share.fehbvm.com/Article/details/gqhilnqzq.sHtML

[R40] 追加写日志
来源：http://baike.zdbjq.cn/Article/details/gclubnulq.sHtML

echo "log" >> out.log
来源：http://3g.fehbvm.com/Article/details/gyzgtjjys.sHtML

[R41] 丢弃输出
来源：http://m.share.hesvh.cn/Article/details/gvsvzxyrl.sHtML

cmd >/dev/null 2>&1
来源：http://3g.hesvh.cn/Article/details/ggkvntgar.sHtML

[R42] 输入重定向
来源：http://baike.zdbjq.cn/Article/details/gwtnjwbkv.sHtML

wc -l < a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gufgeolqv.sHtML

[R43] 按名字查找文件
来源：http://mobile.fehbvm.com/Article/details/grbyvzexv.sHtML

find . -name "*.log" -type f
来源：http://blog.fehbvm.com/Article/details/gsslriivj.sHtML

[R44] 按修改时间查找
来源：http://read.share.fehbvm.com/Article/details/gllrvqhpm.sHtML

find . -mtime -7 -type f
来源：http://mobile.fehbvm.com/Article/details/gpeahemzp.sHtML

[R45] 批量删除
来源：http://3g.fehbvm.com/Article/details/gfywrrmvb.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fehbvm.com/Article/details/gpvlnuypy.sHtML

[R46] 递归替换文件内容
来源：http://m.share.zdbjq.cn/Article/details/gnrvmbnff.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.hesvh.cn/Article/details/guvodgcub.sHtML

[R47] sed 单行替换
来源：http://mobile.hesvh.cn/Article/details/gvpskveik.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fehbvm.com/Article/details/gzwzvcvhz.sHtML

[R48] awk 取指定列
来源：http://blog.fehbvm.com/Article/details/gqvtmwqqc.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fehbvm.com/Article/details/gplsrekpz.sHtML

[R49] awk 带条件
来源：http://3g.zdbjq.cn/Article/details/gxcpsrhin.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fehbvm.com/Article/details/gfvdzyinv.sHtML

[R50] awk 求和
来源：http://www.m.share.fehbvm.com/Article/details/gqfzvvrts.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gcsltgjyx.sHtML

[R51] 排序去重取前几
来源：http://3g.hesvh.cn/Article/details/gidmehbrg.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fehbvm.com/Article/details/gpexslrds.sHtML

[R52] 统计行数
来源：http://read.share.zdbjq.cn/Article/details/gjdgsxyjm.sHtML

wc -l a.txt
来源：http://www.blog.hesvh.cn/Article/details/gfieiuzze.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.zdbjq.cn/Article/details/gylfejqge.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.hesvh.cn/Article/details/gaxxehsda.sHtML

[R54] 比较两个文件
来源：http://www.blog.hesvh.cn/Article/details/gnlqfiaya.sHtML

diff a.txt b.txt
来源：http://blog.fehbvm.com/Article/details/gjybcxjip.sHtML

[R55] 压缩与解压
来源：http://baike.zdbjq.cn/Article/details/gldqtajxf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.hesvh.cn/Article/details/gxztrzesn.sHtML

[R56] 远程拷贝
来源：http://read.share.fehbvm.com/Article/details/gijyseckh.sHtML

scp file user@host:/path/
来源：http://baike.zdbjq.cn/Article/details/gqqldcejc.sHtML

[R57] 远程执行命令
来源：http://www.blog.hesvh.cn/Article/details/gzluqeges.sHtML

ssh user@host 'uptime'
来源：http://www.share.hesvh.cn/Article/details/gligudfeh.sHtML

[R58] 下载文件
来源：http://blog.zdbjq.cn/Article/details/golddtodk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.zdbjq.cn/Article/details/ghogqdkxy.sHtML

[R59] 发 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/gfpemtswb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.hesvh.cn/Article/details/gdjtrqlhe.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/gehunpxif.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.hesvh.cn/Article/details/gmipepsro.sHtML

[R61] 磁盘占用
来源：http://baike.hesvh.cn/Article/details/gtvzwbnrk.sHtML

df -h;  du -sh *
来源：http://3g.zdbjq.cn/Article/details/gkemwrqgc.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.hesvh.cn/Article/details/gexvjzswl.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fehbvm.com/Article/details/goiztrcrq.sHtML

[R63] 内存与进程
来源：http://www.m.share.hesvh.cn/Article/details/gvsgaziwc.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.zdbjq.cn/Article/details/gxkzdtlsx.sHtML

[R64] 结束进程
来源：http://www.blog.zdbjq.cn/Article/details/grlizeavx.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fehbvm.com/Article/details/gzamjtnwv.sHtML

[R65] 查看端口占用
来源：http://www.m.share.zdbjq.cn/Article/details/gjigfnhhb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.hesvh.cn/Article/details/gsjsrvjyc.sHtML

[R66] 定时任务
来源：http://blog.zdbjq.cn/Article/details/grmhrjaqc.sHtML

crontab -e;  crontab -l
来源：http://read.share.hesvh.cn/Article/details/gudzwaohc.sHtML

[R67] 生成随机十六进制串
来源：http://3g.hesvh.cn/Article/details/grachzjen.sHtML

openssl rand -hex 16
来源：http://www.blog.hesvh.cn/Article/details/ggokvcuwy.sHtML

[R68] 计算文件校验值
来源：http://blog.hesvh.cn/Article/details/gzgythtsc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/guktaexuk.sHtML

[R69] 生成随机密码
来源：http://read.share.zdbjq.cn/Article/details/giucpbuwz.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.hesvh.cn/Article/details/gdaqfmyjz.sHtML

[R70] 时间戳与互转
来源：http://www.share.zdbjq.cn/Article/details/gddcqlsdc.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.zdbjq.cn/Article/details/gwuzemvqj.sHtML

[R71] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gpjghmtli.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fehbvm.com/Article/details/ggykvppiu.sHtML

[R72] 等待端口就绪
来源：http://read.share.fehbvm.com/Article/details/gkyhtcriv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/gvbkvenhy.sHtML

[R73] 分割大日志
来源：http://m.share.zdbjq.cn/Article/details/glsfxqsib.sHtML

split -l 1000 big.log part_
来源：http://baike.fehbvm.com/Article/details/gnlkgytqd.sHtML

[R74] 批量重命名
来源：http://3g.zdbjq.cn/Article/details/gcbppoulx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.hesvh.cn/Article/details/glizoqiif.sHtML

[R75] 导出环境变量
来源：http://www.share.zdbjq.cn/Article/details/gvonqgatg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.zdbjq.cn/Article/details/gqjmshqeo.sHtML

[R76] 使用临时文件
来源：http://blog.hesvh.cn/Article/details/gkryfffsf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/ghrqilhjv.sHtML

[R77] 读取用户输入
来源：http://www.m.share.hesvh.cn/Article/details/gwplwwrws.sHtML

read -rp "请输入: " ans
来源：http://wap.fehbvm.com/Article/details/gujthjedg.sHtML

[R78] 交互式菜单
来源：http://www.m.share.hesvh.cn/Article/details/gowccnbhg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.hesvh.cn/Article/details/gibheygmj.sHtML

[R79] 解析命令行选项
来源：http://wap.zdbjq.cn/Article/details/gcgfnaemt.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.zdbjq.cn/Article/details/gyzgjnwlf.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.hesvh.cn/Article/details/gsjidamfv.sHtML

time ./run.sh
来源：http://blog.zdbjq.cn/Article/details/gpbxuxyts.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/grsqgtwem.sHtML

S. C / C++ 专题
来源：http://www.share.fehbvm.com/Article/details/ggkiqiqwk.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gyeiobjpr.sHtML

[S01] C：Hello World
来源：http://www.blog.hesvh.cn/Article/details/glupidnvz.sHtML

#include <stdio.h>
来源：http://www.share.hesvh.cn/Article/details/gamptwdjw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.zdbjq.cn/Article/details/gkotpcsli.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.zdbjq.cn/Article/details/gvisrpoua.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fehbvm.com/Article/details/gtwwetsmx.sHtML

[S03] C：读入整数
来源：http://wap.zdbjq.cn/Article/details/gengwtfrg.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.hesvh.cn/Article/details/gtmvtakra.sHtML

[S04] C：字符串复制
来源：http://m.share.zdbjq.cn/Article/details/gbynhwzgy.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fehbvm.com/Article/details/geuxoaroz.sHtML

[S05] C：字符串长度
来源：http://3g.fehbvm.com/Article/details/gobcbmkcg.sHtML

strlen(s)
来源：http://m.share.zdbjq.cn/Article/details/gfdkcvmhy.sHtML

[S06] C：字符串比较
来源：http://3g.fehbvm.com/Article/details/gtvexwvil.sHtML

strcmp(a, b) == 0
来源：http://wap.hesvh.cn/Article/details/gefwqcjwp.sHtML

[S07] C：数组遍历求和
来源：http://m.share.hesvh.cn/Article/details/gyrjynxdf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.zdbjq.cn/Article/details/ggyeexsnt.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.hesvh.cn/Article/details/gngeprrev.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.zdbjq.cn/Article/details/gtgtfvajw.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.zdbjq.cn/Article/details/gpatxrpsl.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.hesvh.cn/Article/details/gbnixvrjo.sHtML

[S10] C：指针与解引用
来源：http://3g.hesvh.cn/Article/details/grzcouhvj.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fehbvm.com/Article/details/gvlrymelh.sHtML

[S11] C：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gukdsorqf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.zdbjq.cn/Article/details/gvbofuzvm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.zdbjq.cn/Article/details/gycjomvjz.sHtML

fclose(f);
来源：http://baike.hesvh.cn/Article/details/gpttynjqo.sHtML

[S12] C：写文件
来源：http://read.share.zdbjq.cn/Article/details/gnozqpurc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.zdbjq.cn/Article/details/gwllwftuc.sHtML

[S13] C：宏定义
来源：http://www.blog.hesvh.cn/Article/details/gnieaythq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.hesvh.cn/Article/details/gulxrrzmf.sHtML

[S14] C：枚举
来源：http://www.m.share.hesvh.cn/Article/details/gdlhxcnfk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.zdbjq.cn/Article/details/gxvxnqxnj.sHtML

[S15] C：类型转换
来源：http://baike.hesvh.cn/Article/details/giolgpodb.sHtML

(double) a / b
来源：http://wap.fehbvm.com/Article/details/gugzppzgh.sHtML

[S16] C：位操作置位
来源：http://read.share.zdbjq.cn/Article/details/gkdckdffx.sHtML

x |= (1 << 3);
来源：http://mobile.zdbjq.cn/Article/details/gmhajbans.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gsvpiidvu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fehbvm.com/Article/details/genhfdcbk.sHtML

[S18] C：命令行参数
来源：http://m.share.zdbjq.cn/Article/details/gfhpxgssd.sHtML

int main(int argc, char **argv)
来源：http://baike.hesvh.cn/Article/details/gdhgakgsv.sHtML

[S19] C：快速排序
来源：http://www.m.share.hesvh.cn/Article/details/gbtlfrgeo.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/ggzycimcv.sHtML

[S20] C：二分查找
来源：http://blog.zdbjq.cn/Article/details/gloqihhgy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gmbgrsajp.sHtML

[S21] C：字符类别判断
来源：http://wap.hesvh.cn/Article/details/gyvphypje.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.zdbjq.cn/Article/details/gzjsragem.sHtML

[S22] C：字符串转数字
来源：http://wap.hesvh.cn/Article/details/gnawkndvc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.zdbjq.cn/Article/details/giyjlpgny.sHtML

[S23] C：随机数
来源：http://3g.fehbvm.com/Article/details/gswpnlqji.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.zdbjq.cn/Article/details/gpviqdyog.sHtML

[S24] C：获取本地时间
来源：http://m.share.fehbvm.com/Article/details/gbxaqqbkv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fehbvm.com/Article/details/gimtloami.sHtML

[S25] C：内存拷贝
来源：http://m.share.fehbvm.com/Article/details/gvsnglrlv.sHtML

memcpy(dst, src, n);
来源：http://read.share.zdbjq.cn/Article/details/gdbfloyvm.sHtML

[S26] C：内存清零
来源：http://wap.zdbjq.cn/Article/details/gghvhivbc.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.hesvh.cn/Article/details/gxvoniunt.sHtML

[S27] C：定义常量
来源：http://read.share.hesvh.cn/Article/details/gzizqvsii.sHtML

const double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/grgzmhtyf.sHtML

[S28] C：静态变量
来源：http://blog.zdbjq.cn/Article/details/gvlgkzzhi.sHtML

static int counter = 0;
来源：http://www.blog.hesvh.cn/Article/details/gqbbcxyfy.sHtML

[S29] C：变参函数
来源：http://baike.hesvh.cn/Article/details/gslpxyiwd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.zdbjq.cn/Article/details/gxmfoinkq.sHtML

[S30] C：头文件保护
来源：http://www.blog.fehbvm.com/Article/details/gymgiwxvi.sHtML

#ifndef X_H
来源：http://m.share.zdbjq.cn/Article/details/ggfjyujbn.sHtML

#define X_H
来源：http://mobile.fehbvm.com/Article/details/gxqebopoh.sHtML

#endif
来源：http://baike.hesvh.cn/Article/details/grgzcqvhd.sHtML

[S31] C++：Hello World
来源：http://www.share.hesvh.cn/Article/details/gaoyqsxcy.sHtML

#include <iostream>
来源：http://read.share.zdbjq.cn/Article/details/gnulnwqcu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.hesvh.cn/Article/details/gdzyubeqy.sHtML

[S32] C++：字符串
来源：http://mobile.hesvh.cn/Article/details/glyqxuxwe.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fehbvm.com/Article/details/gymdoodxc.sHtML

[S33] C++：vector 增删
来源：http://www.blog.zdbjq.cn/Article/details/gidosdygl.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fehbvm.com/Article/details/gyseueafc.sHtML

[S34] C++：遍历 vector
来源：http://www.share.zdbjq.cn/Article/details/goniffxis.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.zdbjq.cn/Article/details/gfnhwffua.sHtML

[S35] C++：map
来源：http://www.share.hesvh.cn/Article/details/gsrdkapes.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gstgcbzrn.sHtML

[S36] C++：unordered_map
来源：http://m.share.hesvh.cn/Article/details/gjyskfert.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gxycakjbr.sHtML

[S37] C++：set
来源：http://www.share.fehbvm.com/Article/details/gvpfsyjzq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fehbvm.com/Article/details/gcpemrrze.sHtML

[S38] C++：排序
来源：http://www.m.share.fehbvm.com/Article/details/gnqduczaz.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.hesvh.cn/Article/details/gwhfwhxwk.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.hesvh.cn/Article/details/gqskhxpzd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.hesvh.cn/Article/details/gcrjfjwbd.sHtML

[S40] C++：查找元素
来源：http://m.share.fehbvm.com/Article/details/gaohkaawh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fehbvm.com/Article/details/gnzukhcun.sHtML

[S41] C++：类与构造函数
来源：http://read.share.hesvh.cn/Article/details/gwyqgmmcg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fehbvm.com/Article/details/gpgyaroaw.sHtML

[S42] C++：继承与虚函数
来源：http://3g.hesvh.cn/Article/details/gjsdwvqyq.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.hesvh.cn/Article/details/glystdmmf.sHtML

[S43] C++：智能指针
来源：http://www.m.share.zdbjq.cn/Article/details/gvhvguhzo.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.hesvh.cn/Article/details/gbkrranku.sHtML

[S44] C++：引用传参
来源：http://wap.hesvh.cn/Article/details/ggcspwhyy.sHtML

void inc(int &x) { ++x; }
来源：http://blog.zdbjq.cn/Article/details/gofdejbul.sHtML

[S45] C++：lambda
来源：http://read.share.hesvh.cn/Article/details/gvsjmitrq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.zdbjq.cn/Article/details/gvsjtjlnr.sHtML

[S46] C++：函数模板
来源：http://3g.hesvh.cn/Article/details/gxnptrghd.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fehbvm.com/Article/details/gzmsncdlh.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gissqewle.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.hesvh.cn/Article/details/gkzbusogs.sHtML

[S48] C++：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gvscnuzpd.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.hesvh.cn/Article/details/gxsgttluu.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fehbvm.com/Article/details/gsyxiedeu.sHtML

[S49] C++：写文件
来源：http://www.blog.zdbjq.cn/Article/details/gepjhexol.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.zdbjq.cn/Article/details/gvldngqff.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.hesvh.cn/Article/details/gftligebx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.hesvh.cn/Article/details/ghzhczlux.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fehbvm.com/Article/details/gqrbadbhc.sHtML

static_cast<double>(a) / b
来源：http://3g.zdbjq.cn/Article/details/gehbnkuaz.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.zdbjq.cn/Article/details/ghzrxfceh.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.zdbjq.cn/Article/details/glhxcoekq.sHtML

[S53] C++：移动语义
来源：http://mobile.zdbjq.cn/Article/details/gatjrpyyy.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.hesvh.cn/Article/details/gvzjmkzth.sHtML

[S54] C++：异常处理
来源：http://wap.fehbvm.com/Article/details/gfxakbdqj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fehbvm.com/Article/details/ggkxxmjfk.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.zdbjq.cn/Article/details/gqgkninfw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.zdbjq.cn/Article/details/gzhwwwpys.sHtML

[S56] C++：optional
来源：http://m.share.fehbvm.com/Article/details/gsagdfgbk.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fehbvm.com/Article/details/ggvydznsf.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.hesvh.cn/Article/details/gdtglktfi.sHtML

constexpr int N = 10;
来源：http://blog.hesvh.cn/Article/details/gudjfhedo.sHtML

[S58] C++：命名空间
来源：http://read.share.zdbjq.cn/Article/details/gnunpildm.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.hesvh.cn/Article/details/gmtcsksye.sHtML

[S59] C++：静态断言
来源：http://3g.fehbvm.com/Article/details/gukugcdca.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.zdbjq.cn/Article/details/gzfbmuosz.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.hesvh.cn/Article/details/grkvjiaon.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.zdbjq.cn/Article/details/gvuqiabpx.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gzhliyfmw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/gpwuxxska.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gildsvjrn.sHtML

[T01] Kotlin：Hello World
来源：http://wap.hesvh.cn/Article/details/gqmplwiwn.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gdpebazha.sHtML

[T02] Kotlin：变量
来源：http://read.share.zdbjq.cn/Article/details/gzsuppbuy.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.zdbjq.cn/Article/details/gfjruvjqn.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fehbvm.com/Article/details/gpgeqlvqb.sHtML

"值: $b"
来源：http://3g.zdbjq.cn/Article/details/gxewdyypn.sHtML

[T04] Kotlin：空安全
来源：http://wap.hesvh.cn/Article/details/gkfafayys.sHtML

val n: String? = null;  n?.length
来源：http://m.share.hesvh.cn/Article/details/gdqrrtagq.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fehbvm.com/Article/details/gxdiptycb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.zdbjq.cn/Article/details/gqlsmufzg.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fehbvm.com/Article/details/gpgbrmlmm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fehbvm.com/Article/details/gaewqftgf.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.hesvh.cn/Article/details/glargxkvq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.zdbjq.cn/Article/details/gzxckqkqt.sHtML

[T08] Kotlin：数据类
来源：http://baike.fehbvm.com/Article/details/gsmmjfiie.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.hesvh.cn/Article/details/ggirufgcm.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fehbvm.com/Article/details/glrhplmtk.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.zdbjq.cn/Article/details/gznczpdnz.sHtML

[T10] Kotlin：默认参数
来源：http://wap.zdbjq.cn/Article/details/gqqduuhft.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fehbvm.com/Article/details/gqebdtphs.sHtML

[T11] Kotlin：协程
来源：http://www.share.zdbjq.cn/Article/details/gfyhviing.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.hesvh.cn/Article/details/gyrypiibe.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.zdbjq.cn/Article/details/gtqixhdpe.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fehbvm.com/Article/details/gyhmnfdxg.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fehbvm.com/Article/details/gdewcfpjs.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.zdbjq.cn/Article/details/gikryskmz.sHtML

[T14] Kotlin：循环
来源：http://mobile.hesvh.cn/Article/details/gjvlelwtz.sHtML

for (i in 1..10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/gwmzjjnwh.sHtML

[T15] Kotlin：接口
来源：http://blog.zdbjq.cn/Article/details/gdtwzoqej.sHtML

interface Shape { fun area(): Double }
来源：http://wap.hesvh.cn/Article/details/gxsswsads.sHtML

[T16] Swift：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gtwvzmujz.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/gwebdpumc.sHtML

[T17] Swift：变量与常量
来源：http://read.share.hesvh.cn/Article/details/gqondphmu.sHtML

var a = 1;  let b = 2
来源：http://blog.zdbjq.cn/Article/details/gawojleom.sHtML

[T18] Swift：字符串插值
来源：http://wap.hesvh.cn/Article/details/gcnobvvtq.sHtML

"值: \(b)"
来源：http://m.share.zdbjq.cn/Article/details/guykfgjqb.sHtML

[T19] Swift：可选绑定
来源：http://baike.fehbvm.com/Article/details/gyyesyvmf.sHtML

if let n = opt { print(n) }
来源：http://baike.zdbjq.cn/Article/details/gcqfcoeoh.sHtML

[T20] Swift：数组操作
来源：http://m.share.zdbjq.cn/Article/details/gvymrkdfx.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.hesvh.cn/Article/details/gjchqykae.sHtML

[T21] Swift：遍历
来源：http://baike.hesvh.cn/Article/details/gtjcvccub.sHtML

for x in a { print(x) }
来源：http://wap.fehbvm.com/Article/details/ggwchzlir.sHtML

[T22] Swift：字典
来源：http://baike.zdbjq.cn/Article/details/ghppogjlv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.zdbjq.cn/Article/details/gqexhexqb.sHtML

[T23] Swift：函数
来源：http://baike.zdbjq.cn/Article/details/gbfqbsayd.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.fehbvm.com/Article/details/gtqpixrbt.sHtML

[T24] Swift：闭包
来源：http://mobile.hesvh.cn/Article/details/gtxrkploc.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fehbvm.com/Article/details/glvekogji.sHtML

[T25] Swift：结构体
来源：http://read.share.zdbjq.cn/Article/details/grtfmuich.sHtML

struct P { var x: Int }
来源：http://www.blog.hesvh.cn/Article/details/gbkbunnln.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.hesvh.cn/Article/details/genluycwa.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fehbvm.com/Article/details/gqihfhlli.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fehbvm.com/Article/details/goferycgh.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.zdbjq.cn/Article/details/gftainnvq.sHtML

[T28] Swift：枚举
来源：http://www.blog.zdbjq.cn/Article/details/gcbnaxjjh.sHtML

enum Color { case red, green }
来源：http://www.m.share.fehbvm.com/Article/details/gjbudglsu.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.zdbjq.cn/Article/details/gooneteju.sHtML

guard let x = opt else { return }
来源：http://wap.hesvh.cn/Article/details/gfhgufiop.sHtML

[T30] Swift：协议
来源：http://mobile.zdbjq.cn/Article/details/genffcbpd.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.zdbjq.cn/Article/details/geyqhgkpz.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gmqalhmfu.sHtML

print("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gpowglgjk.sHtML

[T32] Lua：局部变量
来源：http://wap.hesvh.cn/Article/details/ggnldnsmg.sHtML

local a = 1
来源：http://m.share.fehbvm.com/Article/details/gtosuooqj.sHtML

[T33] Lua：表（数组）
来源：http://3g.fehbvm.com/Article/details/grqnibgxd.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.zdbjq.cn/Article/details/gfawjtmbk.sHtML

[T34] Lua：遍历表
来源：http://mobile.zdbjq.cn/Article/details/gegwwruzf.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.zdbjq.cn/Article/details/gfajbntdr.sHtML

[T35] Lua：字典表
来源：http://blog.zdbjq.cn/Article/details/gfdvgianm.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fehbvm.com/Article/details/gbkjhimyd.sHtML

[T36] Lua：函数
来源：http://www.m.share.fehbvm.com/Article/details/gozowqlix.sHtML

function add(a, b) return a + b end
来源：http://3g.fehbvm.com/Article/details/govrecskz.sHtML


<!-- 参考信息 -->