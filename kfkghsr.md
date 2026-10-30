代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.zdbjq.cn/Article/details/gjidanbmt.sHtML

[R30] 函数返回状态码
来源：http://www.share.fehbvm.com/Article/details/geznmptub.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.hesvh.cn/Article/details/gtwsvieua.sHtML

[R31] 局部变量
来源：http://mobile.fehbvm.com/Article/details/gpturlrty.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsvisxiqy.sHtML

[R32] 参数个数校验
来源：http://www.blog.zdbjq.cn/Article/details/gmubqrlmc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/gyctmnssw.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.zdbjq.cn/Article/details/gfylqbuxo.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.zdbjq.cn/Article/details/ggvhkaenw.sHtML

[R34] 退出时清理
来源：http://m.share.hesvh.cn/Article/details/gdypjfwad.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gwbofwelm.sHtML

[R35] 后台执行并等待
来源：http://wap.fehbvm.com/Article/details/gkijxjnvp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.hesvh.cn/Article/details/glpzlxkig.sHtML

[R36] 并发执行多个任务
来源：http://www.share.hesvh.cn/Article/details/gymtfjsjy.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.hesvh.cn/Article/details/gmensyvup.sHtML

[R37] 把输出赋给变量
来源：http://blog.fehbvm.com/Article/details/gowjinpxg.sHtML

files=$(ls -1)
来源：http://baike.hesvh.cn/Article/details/gaswhmuts.sHtML

[R38] 管道串联
来源：http://mobile.zdbjq.cn/Article/details/grlxtrenm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.hesvh.cn/Article/details/glwlfengw.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fehbvm.com/Article/details/ghboxexen.sHtML

cmd > out.log 2>&1
来源：http://www.share.hesvh.cn/Article/details/gkpfjypme.sHtML

[R40] 追加写日志
来源：http://www.m.share.hesvh.cn/Article/details/gzcvwcsyo.sHtML

echo "log" >> out.log
来源：http://3g.hesvh.cn/Article/details/goifdqvdm.sHtML

[R41] 丢弃输出
来源：http://www.blog.zdbjq.cn/Article/details/gmmobblly.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/gbykckjlf.sHtML

[R42] 输入重定向
来源：http://www.blog.hesvh.cn/Article/details/gabuokjzx.sHtML

wc -l < a.txt
来源：http://mobile.zdbjq.cn/Article/details/gqnywwtux.sHtML

[R43] 按名字查找文件
来源：http://wap.hesvh.cn/Article/details/gymojycsp.sHtML

find . -name "*.log" -type f
来源：http://www.blog.hesvh.cn/Article/details/gossbqtgh.sHtML

[R44] 按修改时间查找
来源：http://3g.hesvh.cn/Article/details/gqolxxnrf.sHtML

find . -mtime -7 -type f
来源：http://3g.fehbvm.com/Article/details/ghmpxxpoh.sHtML

[R45] 批量删除
来源：http://mobile.fehbvm.com/Article/details/gvxcxodib.sHtML

find . -name "*.tmp" -delete
来源：http://3g.hesvh.cn/Article/details/girywgctq.sHtML

[R46] 递归替换文件内容
来源：http://www.share.hesvh.cn/Article/details/guhbyfoco.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.zdbjq.cn/Article/details/gtujppcvx.sHtML

[R47] sed 单行替换
来源：http://www.share.hesvh.cn/Article/details/gpgthaxkw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.hesvh.cn/Article/details/gwadacypk.sHtML

[R48] awk 取指定列
来源：http://www.m.share.zdbjq.cn/Article/details/gmmqllsat.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.hesvh.cn/Article/details/gipjjojpd.sHtML

[R49] awk 带条件
来源：http://www.blog.zdbjq.cn/Article/details/goqowndup.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.hesvh.cn/Article/details/gqsgrroyy.sHtML

[R50] awk 求和
来源：http://www.share.zdbjq.cn/Article/details/gsfezeeal.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fehbvm.com/Article/details/gipzfemaq.sHtML

[R51] 排序去重取前几
来源：http://read.share.hesvh.cn/Article/details/gxfewkakh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.zdbjq.cn/Article/details/ggyowkxjc.sHtML

[R52] 统计行数
来源：http://www.m.share.fehbvm.com/Article/details/grrvpbkuw.sHtML

wc -l a.txt
来源：http://www.blog.hesvh.cn/Article/details/ghbgpylzf.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fehbvm.com/Article/details/gdvarmsmc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.zdbjq.cn/Article/details/ggxgbhihq.sHtML

[R54] 比较两个文件
来源：http://blog.fehbvm.com/Article/details/gddojubsz.sHtML

diff a.txt b.txt
来源：http://mobile.hesvh.cn/Article/details/grerqowzn.sHtML

[R55] 压缩与解压
来源：http://3g.hesvh.cn/Article/details/gkakrrbvu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.zdbjq.cn/Article/details/gjhoqgbcz.sHtML

[R56] 远程拷贝
来源：http://wap.hesvh.cn/Article/details/ggchuyzex.sHtML

scp file user@host:/path/
来源：http://3g.zdbjq.cn/Article/details/gmzyzyqvh.sHtML

[R57] 远程执行命令
来源：http://3g.zdbjq.cn/Article/details/grzqxqsdf.sHtML

ssh user@host 'uptime'
来源：http://read.share.hesvh.cn/Article/details/gymhikfsm.sHtML

[R58] 下载文件
来源：http://m.share.fehbvm.com/Article/details/gcjxsdzwp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.hesvh.cn/Article/details/griibydvc.sHtML

[R59] 发 POST JSON
来源：http://m.share.hesvh.cn/Article/details/gnwdvuxne.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.zdbjq.cn/Article/details/gdxprvuxn.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/gvcawffuh.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.hesvh.cn/Article/details/gtnswfjbi.sHtML

[R61] 磁盘占用
来源：http://www.share.fehbvm.com/Article/details/ggwiqzgzm.sHtML

df -h;  du -sh *
来源：http://mobile.fehbvm.com/Article/details/gvlqdeagv.sHtML

[R62] 找最占空间的文件
来源：http://baike.fehbvm.com/Article/details/gjchbffbe.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fehbvm.com/Article/details/gdczrobyd.sHtML

[R63] 内存与进程
来源：http://baike.zdbjq.cn/Article/details/gevodeigw.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.hesvh.cn/Article/details/gcqmtcmth.sHtML

[R64] 结束进程
来源：http://www.m.share.zdbjq.cn/Article/details/gnjmhcehg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.hesvh.cn/Article/details/ggtvmbstz.sHtML

[R65] 查看端口占用
来源：http://m.share.hesvh.cn/Article/details/gnddondmx.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.hesvh.cn/Article/details/gfpzbjoqo.sHtML

[R66] 定时任务
来源：http://www.m.share.hesvh.cn/Article/details/gipqtexet.sHtML

crontab -e;  crontab -l
来源：http://www.share.zdbjq.cn/Article/details/gczfqtaau.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.zdbjq.cn/Article/details/gjbvqlktx.sHtML

openssl rand -hex 16
来源：http://baike.fehbvm.com/Article/details/geivecwnd.sHtML

[R68] 计算文件校验值
来源：http://mobile.zdbjq.cn/Article/details/gniahsnkp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.zdbjq.cn/Article/details/gfsnkmqlx.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fehbvm.com/Article/details/gfsvkmzly.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.hesvh.cn/Article/details/gfayldlnc.sHtML

[R70] 时间戳与互转
来源：http://read.share.hesvh.cn/Article/details/gnmwqrfnl.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.zdbjq.cn/Article/details/gzqjlvbop.sHtML

[R71] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/gmtahgchl.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fehbvm.com/Article/details/gudagzwgh.sHtML

[R72] 等待端口就绪
来源：http://wap.zdbjq.cn/Article/details/gtpcvcfjj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/glnjnxznq.sHtML

[R73] 分割大日志
来源：http://3g.fehbvm.com/Article/details/ghozekvio.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.zdbjq.cn/Article/details/grirvuguy.sHtML

[R74] 批量重命名
来源：http://3g.fehbvm.com/Article/details/gnusvpqmw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fehbvm.com/Article/details/geoiesyic.sHtML

[R75] 导出环境变量
来源：http://3g.zdbjq.cn/Article/details/gysguihxw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fehbvm.com/Article/details/gtjccmooz.sHtML

[R76] 使用临时文件
来源：http://read.share.hesvh.cn/Article/details/geohbeklx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gclexpzmk.sHtML

[R77] 读取用户输入
来源：http://m.share.hesvh.cn/Article/details/gzboutldt.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fehbvm.com/Article/details/gajdbqicr.sHtML

[R78] 交互式菜单
来源：http://www.share.fehbvm.com/Article/details/gtjtezsbu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fehbvm.com/Article/details/gvsqjmjsk.sHtML

[R79] 解析命令行选项
来源：http://3g.hesvh.cn/Article/details/ghzlmqylz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.zdbjq.cn/Article/details/gbzzqbxos.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fehbvm.com/Article/details/gwmuemwgv.sHtML

time ./run.sh
来源：http://read.share.zdbjq.cn/Article/details/gixehjudu.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gcitwqpxb.sHtML

S. C / C++ 专题
来源：http://read.share.hesvh.cn/Article/details/gfmdosnao.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gvhxuehod.sHtML

[S01] C：Hello World
来源：http://3g.fehbvm.com/Article/details/gpjiawgds.sHtML

#include <stdio.h>
来源：http://blog.hesvh.cn/Article/details/gupctkzrk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.zdbjq.cn/Article/details/gihwhrlxu.sHtML

[S02] C：变量与格式化输出
来源：http://baike.hesvh.cn/Article/details/gzxohxcjs.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fehbvm.com/Article/details/gsjlbgsrt.sHtML

[S03] C：读入整数
来源：http://m.share.fehbvm.com/Article/details/gdwrsnnpc.sHtML

int x; scanf("%d", &x);
来源：http://baike.hesvh.cn/Article/details/gggiuedss.sHtML

[S04] C：字符串复制
来源：http://read.share.hesvh.cn/Article/details/ggibkbbpw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fehbvm.com/Article/details/gvhqvcrxs.sHtML

[S05] C：字符串长度
来源：http://wap.hesvh.cn/Article/details/grfyihmul.sHtML

strlen(s)
来源：http://3g.zdbjq.cn/Article/details/gljswuwel.sHtML

[S06] C：字符串比较
来源：http://wap.hesvh.cn/Article/details/gssempevf.sHtML

strcmp(a, b) == 0
来源：http://baike.zdbjq.cn/Article/details/gxqnqoqcg.sHtML

[S07] C：数组遍历求和
来源：http://mobile.hesvh.cn/Article/details/gbgunfpbt.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.hesvh.cn/Article/details/gvasmeczy.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.hesvh.cn/Article/details/giyldwoft.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.zdbjq.cn/Article/details/gtaidpbsa.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.zdbjq.cn/Article/details/gxmabrzye.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.hesvh.cn/Article/details/gzjzwqpzb.sHtML

[S10] C：指针与解引用
来源：http://mobile.fehbvm.com/Article/details/gmibnywmo.sHtML

int *p = &a;  *p = 5;
来源：http://baike.zdbjq.cn/Article/details/gutelitdx.sHtML

[S11] C：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gwuylzbps.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fehbvm.com/Article/details/ghfoygjqa.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.zdbjq.cn/Article/details/gqmgnjlhl.sHtML

fclose(f);
来源：http://blog.fehbvm.com/Article/details/gqusdnmzd.sHtML

[S12] C：写文件
来源：http://m.share.fehbvm.com/Article/details/gdpmzbntc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fehbvm.com/Article/details/gjhnymtdc.sHtML

[S13] C：宏定义
来源：http://3g.hesvh.cn/Article/details/gttpqagch.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fehbvm.com/Article/details/gcwstqmqw.sHtML

[S14] C：枚举
来源：http://wap.hesvh.cn/Article/details/gicyncnne.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.hesvh.cn/Article/details/gieucqazb.sHtML

[S15] C：类型转换
来源：http://3g.fehbvm.com/Article/details/gfecgabbh.sHtML

(double) a / b
来源：http://www.m.share.hesvh.cn/Article/details/gzhgslhbo.sHtML

[S16] C：位操作置位
来源：http://m.share.fehbvm.com/Article/details/gasqjhtjg.sHtML

x |= (1 << 3);
来源：http://read.share.zdbjq.cn/Article/details/gfbcaqsrj.sHtML

[S17] C：安全拼接字符串
来源：http://wap.hesvh.cn/Article/details/gcsnmkpeo.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.hesvh.cn/Article/details/gesvphgxx.sHtML

[S18] C：命令行参数
来源：http://mobile.zdbjq.cn/Article/details/gwbslfypk.sHtML

int main(int argc, char **argv)
来源：http://www.share.fehbvm.com/Article/details/gwokvdmoe.sHtML

[S19] C：快速排序
来源：http://m.share.zdbjq.cn/Article/details/gmtmsgetm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gzxurxagi.sHtML

[S20] C：二分查找
来源：http://blog.zdbjq.cn/Article/details/gnmfszasy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/gjyjqnnow.sHtML

[S21] C：字符类别判断
来源：http://m.share.fehbvm.com/Article/details/gylsbzrvd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.hesvh.cn/Article/details/gqftjmebf.sHtML

[S22] C：字符串转数字
来源：http://m.share.hesvh.cn/Article/details/goytrdker.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.zdbjq.cn/Article/details/gbyydramp.sHtML

[S23] C：随机数
来源：http://www.m.share.hesvh.cn/Article/details/gyxudbpdt.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.hesvh.cn/Article/details/gluokleso.sHtML

[S24] C：获取本地时间
来源：http://mobile.zdbjq.cn/Article/details/gbitmykwr.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.hesvh.cn/Article/details/gorsrujri.sHtML

[S25] C：内存拷贝
来源：http://www.share.zdbjq.cn/Article/details/glnohnbbz.sHtML

memcpy(dst, src, n);
来源：http://mobile.zdbjq.cn/Article/details/griuhosdw.sHtML

[S26] C：内存清零
来源：http://www.share.fehbvm.com/Article/details/gtwnkjuhy.sHtML

memset(a, 0, sizeof a);
来源：http://blog.hesvh.cn/Article/details/gymqyrocu.sHtML

[S27] C：定义常量
来源：http://mobile.hesvh.cn/Article/details/gnyodvgyf.sHtML

const double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gbwaqkdvq.sHtML

[S28] C：静态变量
来源：http://www.m.share.fehbvm.com/Article/details/glgqyimoq.sHtML

static int counter = 0;
来源：http://wap.hesvh.cn/Article/details/ghkplfoyj.sHtML

[S29] C：变参函数
来源：http://www.share.hesvh.cn/Article/details/giiobmhbo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fehbvm.com/Article/details/geuymhjrv.sHtML

[S30] C：头文件保护
来源：http://blog.fehbvm.com/Article/details/gguqhfxas.sHtML

#ifndef X_H
来源：http://mobile.fehbvm.com/Article/details/gvnqlzqht.sHtML

#define X_H
来源：http://read.share.fehbvm.com/Article/details/gskjcgtnp.sHtML

#endif
来源：http://wap.hesvh.cn/Article/details/gdmqqokoc.sHtML

[S31] C++：Hello World
来源：http://wap.hesvh.cn/Article/details/gvokjlmtz.sHtML

#include <iostream>
来源：http://m.share.fehbvm.com/Article/details/gabhtvuik.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.zdbjq.cn/Article/details/gzfysfjxu.sHtML

[S32] C++：字符串
来源：http://www.blog.zdbjq.cn/Article/details/govaskmvn.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.hesvh.cn/Article/details/gedztzdcg.sHtML

[S33] C++：vector 增删
来源：http://m.share.fehbvm.com/Article/details/gioifgzvr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.zdbjq.cn/Article/details/gyrzrwill.sHtML

[S34] C++：遍历 vector
来源：http://blog.zdbjq.cn/Article/details/gzptmvaob.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.zdbjq.cn/Article/details/gqatshphf.sHtML

[S35] C++：map
来源：http://www.blog.zdbjq.cn/Article/details/gawumhgwv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gdxoanulq.sHtML

[S36] C++：unordered_map
来源：http://m.share.hesvh.cn/Article/details/geewubkce.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gubzrbrvh.sHtML

[S37] C++：set
来源：http://3g.zdbjq.cn/Article/details/gfavinhlh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fehbvm.com/Article/details/ghzsuqeyh.sHtML

[S38] C++：排序
来源：http://read.share.fehbvm.com/Article/details/geqclonvg.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.hesvh.cn/Article/details/gjwkbjmrp.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.hesvh.cn/Article/details/gncddizbt.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.zdbjq.cn/Article/details/giwnpyeuu.sHtML

[S40] C++：查找元素
来源：http://wap.hesvh.cn/Article/details/gjsijudpj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fehbvm.com/Article/details/gnfiirfjz.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fehbvm.com/Article/details/glfauriyt.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fehbvm.com/Article/details/gudwbpvrv.sHtML

[S42] C++：继承与虚函数
来源：http://blog.hesvh.cn/Article/details/gygrynzlb.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.zdbjq.cn/Article/details/ghymawyyy.sHtML

[S43] C++：智能指针
来源：http://www.share.zdbjq.cn/Article/details/gbcmmthgv.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.zdbjq.cn/Article/details/glnmeyzss.sHtML

[S44] C++：引用传参
来源：http://3g.fehbvm.com/Article/details/gptynjmhy.sHtML

void inc(int &x) { ++x; }
来源：http://baike.zdbjq.cn/Article/details/gaacopgii.sHtML

[S45] C++：lambda
来源：http://www.m.share.fehbvm.com/Article/details/guqtkntes.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.hesvh.cn/Article/details/gjhtedwwi.sHtML

[S46] C++：函数模板
来源：http://www.blog.zdbjq.cn/Article/details/gzxbwpwze.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.hesvh.cn/Article/details/gjyztzdle.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.zdbjq.cn/Article/details/gdliphpat.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.zdbjq.cn/Article/details/gvpadlxdp.sHtML

[S48] C++：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/ghuiccors.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.hesvh.cn/Article/details/grsmggkoi.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.zdbjq.cn/Article/details/gcvcueuoe.sHtML

[S49] C++：写文件
来源：http://www.m.share.zdbjq.cn/Article/details/gnkhpfkhd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.hesvh.cn/Article/details/gorsbxuuf.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fehbvm.com/Article/details/gzvzhmzeg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gnizkmeph.sHtML

[S51] C++：显式类型转换
来源：http://3g.zdbjq.cn/Article/details/grmyhpbjk.sHtML

static_cast<double>(a) / b
来源：http://blog.zdbjq.cn/Article/details/grosackdq.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.hesvh.cn/Article/details/gxzkfssxk.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fehbvm.com/Article/details/goradvlxt.sHtML

[S53] C++：移动语义
来源：http://read.share.fehbvm.com/Article/details/gipyfoucm.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.hesvh.cn/Article/details/gwjinnaru.sHtML

[S54] C++：异常处理
来源：http://baike.zdbjq.cn/Article/details/gzncetqlj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fehbvm.com/Article/details/gcutyvhgu.sHtML

[S55] C++：结构化绑定
来源：http://blog.zdbjq.cn/Article/details/gourkurgw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fehbvm.com/Article/details/gmxdtteao.sHtML

[S56] C++：optional
来源：http://m.share.zdbjq.cn/Article/details/grwegykvg.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.zdbjq.cn/Article/details/gmizrwbnf.sHtML

[S57] C++：编译期常量
来源：http://www.share.fehbvm.com/Article/details/gvddghlch.sHtML

constexpr int N = 10;
来源：http://m.share.fehbvm.com/Article/details/gzhvhdymr.sHtML

[S58] C++：命名空间
来源：http://blog.fehbvm.com/Article/details/gbhkjoxym.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.hesvh.cn/Article/details/glfkrdxcx.sHtML

[S59] C++：静态断言
来源：http://www.m.share.zdbjq.cn/Article/details/gaumtjlla.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.zdbjq.cn/Article/details/gfomhhbjt.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.zdbjq.cn/Article/details/gkjwqvwpa.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.zdbjq.cn/Article/details/givhpdqhc.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gvboghjft.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fehbvm.com/Article/details/gvgevxjhv.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gtfwnwusd.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gnujiqdod.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/gsifxjlll.sHtML

[T02] Kotlin：变量
来源：http://wap.fehbvm.com/Article/details/gstihdkos.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.hesvh.cn/Article/details/gzyuwkppi.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fehbvm.com/Article/details/gqyykwump.sHtML

"值: $b"
来源：http://www.share.fehbvm.com/Article/details/ghwnpvach.sHtML

[T04] Kotlin：空安全
来源：http://blog.fehbvm.com/Article/details/gbkwnwqgs.sHtML

val n: String? = null;  n?.length
来源：http://m.share.zdbjq.cn/Article/details/gapbmruun.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.hesvh.cn/Article/details/gwjzrdzco.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.zdbjq.cn/Article/details/gmaxlwcgy.sHtML

[T06] Kotlin：集合映射
来源：http://3g.hesvh.cn/Article/details/giaxmxrwj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/ggwdzmxyo.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.hesvh.cn/Article/details/gggmcyehv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fehbvm.com/Article/details/gmyqeoirk.sHtML

[T08] Kotlin：数据类
来源：http://m.share.zdbjq.cn/Article/details/gkhgoxqjd.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.hesvh.cn/Article/details/gfhwfvtba.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.zdbjq.cn/Article/details/gpuogfomo.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fehbvm.com/Article/details/godhqucau.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.hesvh.cn/Article/details/ggrqoeqkm.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.hesvh.cn/Article/details/guooecser.sHtML

[T11] Kotlin：协程
来源：http://blog.zdbjq.cn/Article/details/glnzzdojk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fehbvm.com/Article/details/goazzssid.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fehbvm.com/Article/details/glabciipr.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gasjyfqde.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.zdbjq.cn/Article/details/gcbvwgrvu.sHtML

val m = mapOf("a" to 1)
来源：http://wap.zdbjq.cn/Article/details/gukwvsbry.sHtML

[T14] Kotlin：循环
来源：http://read.share.fehbvm.com/Article/details/gtptzhqhi.sHtML

for (i in 1..10) println(i)
来源：http://blog.zdbjq.cn/Article/details/gjgqregrh.sHtML

[T15] Kotlin：接口
来源：http://3g.zdbjq.cn/Article/details/gunhkfops.sHtML

interface Shape { fun area(): Double }
来源：http://wap.hesvh.cn/Article/details/gzhhdkmqt.sHtML

[T16] Swift：Hello World
来源：http://blog.fehbvm.com/Article/details/gtocbxjdv.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/gvhbgwdmd.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fehbvm.com/Article/details/gczqarzry.sHtML

var a = 1;  let b = 2
来源：http://blog.zdbjq.cn/Article/details/gqozfdbdb.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gcralxeob.sHtML

"值: \(b)"
来源：http://wap.zdbjq.cn/Article/details/gsyvubphl.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.zdbjq.cn/Article/details/gvnnqmmkg.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.zdbjq.cn/Article/details/grnwlzphy.sHtML

[T20] Swift：数组操作
来源：http://read.share.fehbvm.com/Article/details/gvedcydea.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.zdbjq.cn/Article/details/gvosbvgwj.sHtML

[T21] Swift：遍历
来源：http://wap.fehbvm.com/Article/details/gxitbncbj.sHtML

for x in a { print(x) }
来源：http://read.share.fehbvm.com/Article/details/gssgwbkqz.sHtML

[T22] Swift：字典
来源：http://3g.zdbjq.cn/Article/details/gjuuooqgp.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fehbvm.com/Article/details/ghijujlsm.sHtML

[T23] Swift：函数
来源：http://m.share.zdbjq.cn/Article/details/gujuulnrj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.hesvh.cn/Article/details/gzndxfrrg.sHtML

[T24] Swift：闭包
来源：http://www.blog.fehbvm.com/Article/details/gslrtjefu.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gpeifztxa.sHtML

[T25] Swift：结构体
来源：http://www.share.zdbjq.cn/Article/details/glyiluynx.sHtML

struct P { var x: Int }
来源：http://baike.hesvh.cn/Article/details/gmxiuggfv.sHtML

[T26] Swift：类与重写
来源：http://wap.zdbjq.cn/Article/details/gzayusnre.sHtML

class A: Base { override func f() {} }
来源：http://baike.zdbjq.cn/Article/details/gxozeljpj.sHtML

[T27] Swift：错误处理
来源：http://mobile.hesvh.cn/Article/details/gcivaihsj.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.zdbjq.cn/Article/details/gfaprqilx.sHtML

[T28] Swift：枚举
来源：http://m.share.zdbjq.cn/Article/details/gssgjfoqr.sHtML

enum Color { case red, green }
来源：http://3g.hesvh.cn/Article/details/gyxkypwfw.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.zdbjq.cn/Article/details/gdwaftmvp.sHtML

guard let x = opt else { return }
来源：http://www.blog.hesvh.cn/Article/details/gllutmmjp.sHtML

[T30] Swift：协议
来源：http://read.share.fehbvm.com/Article/details/gkrviupnh.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fehbvm.com/Article/details/gooykewip.sHtML

[T31] Lua：Hello World
来源：http://m.share.fehbvm.com/Article/details/gunzodlhd.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/gzromhpig.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.hesvh.cn/Article/details/goctzeuwt.sHtML

local a = 1
来源：http://www.blog.zdbjq.cn/Article/details/ghtlupdnw.sHtML


<!-- 参考信息 -->