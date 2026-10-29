代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://wap.fehbvm.com/Article/details/gjfcxnhgq.sHtML

[R32] 参数个数校验
来源：http://read.share.zdbjq.cn/Article/details/gboxxgczy.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/gaixgdmxv.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fehbvm.com/Article/details/gjexhzdvp.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.zdbjq.cn/Article/details/ggpipcvgj.sHtML

[R34] 退出时清理
来源：http://m.share.fehbvm.com/Article/details/gzbapfikk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gywdaztij.sHtML

[R35] 后台执行并等待
来源：http://mobile.hesvh.cn/Article/details/gfyazbbgk.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fehbvm.com/Article/details/gxrntvxwj.sHtML

[R36] 并发执行多个任务
来源：http://m.share.hesvh.cn/Article/details/gkcmntoga.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.zdbjq.cn/Article/details/gibpraiud.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fehbvm.com/Article/details/gollmodiw.sHtML

files=$(ls -1)
来源：http://www.blog.hesvh.cn/Article/details/ggyfwudvd.sHtML

[R38] 管道串联
来源：http://www.blog.fehbvm.com/Article/details/gzzvvndbe.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.zdbjq.cn/Article/details/gutgjqusl.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.zdbjq.cn/Article/details/gsuchfyuf.sHtML

cmd > out.log 2>&1
来源：http://read.share.hesvh.cn/Article/details/gxezgppig.sHtML

[R40] 追加写日志
来源：http://mobile.fehbvm.com/Article/details/gfkghrmnq.sHtML

echo "log" >> out.log
来源：http://baike.zdbjq.cn/Article/details/gzmuwvilr.sHtML

[R41] 丢弃输出
来源：http://m.share.hesvh.cn/Article/details/gcskofufc.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.hesvh.cn/Article/details/gqybpygov.sHtML

[R42] 输入重定向
来源：http://www.blog.fehbvm.com/Article/details/gvgctauqy.sHtML

wc -l < a.txt
来源：http://wap.fehbvm.com/Article/details/gylckvjis.sHtML

[R43] 按名字查找文件
来源：http://wap.zdbjq.cn/Article/details/gjfmyshpo.sHtML

find . -name "*.log" -type f
来源：http://baike.hesvh.cn/Article/details/ggswwxupe.sHtML

[R44] 按修改时间查找
来源：http://baike.zdbjq.cn/Article/details/gpkpovhbb.sHtML

find . -mtime -7 -type f
来源：http://baike.zdbjq.cn/Article/details/ggllwcyqi.sHtML

[R45] 批量删除
来源：http://www.m.share.zdbjq.cn/Article/details/grkhzxhkf.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.hesvh.cn/Article/details/gaqqbijlp.sHtML

[R46] 递归替换文件内容
来源：http://baike.zdbjq.cn/Article/details/gtmimeegz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fehbvm.com/Article/details/gyvnteuod.sHtML

[R47] sed 单行替换
来源：http://blog.zdbjq.cn/Article/details/gtmcnbfpu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fehbvm.com/Article/details/ggluievkv.sHtML

[R48] awk 取指定列
来源：http://www.share.hesvh.cn/Article/details/gzxkrsmaf.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gmcapmxoc.sHtML

[R49] awk 带条件
来源：http://mobile.fehbvm.com/Article/details/gvxqubjsu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.hesvh.cn/Article/details/guqbagxrs.sHtML

[R50] awk 求和
来源：http://baike.hesvh.cn/Article/details/gctckdxvf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gvietihfx.sHtML

[R51] 排序去重取前几
来源：http://read.share.fehbvm.com/Article/details/guahzecfm.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fehbvm.com/Article/details/govuuhjcl.sHtML

[R52] 统计行数
来源：http://blog.hesvh.cn/Article/details/gxhqnhlfb.sHtML

wc -l a.txt
来源：http://mobile.hesvh.cn/Article/details/gfolochdv.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fehbvm.com/Article/details/gjhxxegwx.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.hesvh.cn/Article/details/gwgukitzq.sHtML

[R54] 比较两个文件
来源：http://blog.fehbvm.com/Article/details/gscrafiik.sHtML

diff a.txt b.txt
来源：http://www.share.hesvh.cn/Article/details/gfsfycztl.sHtML

[R55] 压缩与解压
来源：http://3g.fehbvm.com/Article/details/gffmngkst.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fehbvm.com/Article/details/glvtmrjny.sHtML

[R56] 远程拷贝
来源：http://baike.fehbvm.com/Article/details/gjgwuszhe.sHtML

scp file user@host:/path/
来源：http://blog.fehbvm.com/Article/details/gikrxioll.sHtML

[R57] 远程执行命令
来源：http://baike.fehbvm.com/Article/details/gwmwdjzph.sHtML

ssh user@host 'uptime'
来源：http://www.share.zdbjq.cn/Article/details/gfzjqgepa.sHtML

[R58] 下载文件
来源：http://m.share.zdbjq.cn/Article/details/gpezsgxey.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fehbvm.com/Article/details/glqtlytog.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gxarpgpsj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.hesvh.cn/Article/details/gxhticpsi.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/gibfmnopl.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.hesvh.cn/Article/details/glocxpclt.sHtML

[R61] 磁盘占用
来源：http://m.share.zdbjq.cn/Article/details/gyermzyuu.sHtML

df -h;  du -sh *
来源：http://m.share.hesvh.cn/Article/details/gapminrfn.sHtML

[R62] 找最占空间的文件
来源：http://m.share.zdbjq.cn/Article/details/gjhdtufla.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.hesvh.cn/Article/details/ghvblfcud.sHtML

[R63] 内存与进程
来源：http://wap.fehbvm.com/Article/details/gksotszui.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.zdbjq.cn/Article/details/gossbtfpg.sHtML

[R64] 结束进程
来源：http://m.share.fehbvm.com/Article/details/gfzofklde.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.zdbjq.cn/Article/details/gvqdmelkq.sHtML

[R65] 查看端口占用
来源：http://read.share.fehbvm.com/Article/details/gzfagexex.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.hesvh.cn/Article/details/gngmhsira.sHtML

[R66] 定时任务
来源：http://blog.fehbvm.com/Article/details/gwwxawley.sHtML

crontab -e;  crontab -l
来源：http://blog.zdbjq.cn/Article/details/gohdbqkgf.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.zdbjq.cn/Article/details/ggxsgejxx.sHtML

openssl rand -hex 16
来源：http://www.blog.zdbjq.cn/Article/details/gcqdkuvnu.sHtML

[R68] 计算文件校验值
来源：http://mobile.fehbvm.com/Article/details/gteofazbb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fehbvm.com/Article/details/ghobdwtab.sHtML

[R69] 生成随机密码
来源：http://wap.zdbjq.cn/Article/details/gasckphyt.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.zdbjq.cn/Article/details/ggwpgxmld.sHtML

[R70] 时间戳与互转
来源：http://3g.zdbjq.cn/Article/details/gyvcrvanq.sHtML

date +%s;  date -d @1700000000
来源：http://baike.zdbjq.cn/Article/details/gymlsjahq.sHtML

[R71] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gmzblvddi.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fehbvm.com/Article/details/gpupofybn.sHtML

[R72] 等待端口就绪
来源：http://3g.hesvh.cn/Article/details/gwibqjoel.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/gycznfjgv.sHtML

[R73] 分割大日志
来源：http://baike.fehbvm.com/Article/details/gvzrgxmcl.sHtML

split -l 1000 big.log part_
来源：http://wap.hesvh.cn/Article/details/gyyvcfmjk.sHtML

[R74] 批量重命名
来源：http://mobile.fehbvm.com/Article/details/gmzkcvtpu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.hesvh.cn/Article/details/gymcrfofq.sHtML

[R75] 导出环境变量
来源：http://blog.zdbjq.cn/Article/details/ggujaffdv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.zdbjq.cn/Article/details/gqcwxpnfr.sHtML

[R76] 使用临时文件
来源：http://www.m.share.zdbjq.cn/Article/details/gedvcuykd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/gkfipahdt.sHtML

[R77] 读取用户输入
来源：http://blog.hesvh.cn/Article/details/gtxetlqrc.sHtML

read -rp "请输入: " ans
来源：http://wap.zdbjq.cn/Article/details/gxzvsjofm.sHtML

[R78] 交互式菜单
来源：http://www.blog.hesvh.cn/Article/details/gjtckvufu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.zdbjq.cn/Article/details/gywwtyhjj.sHtML

[R79] 解析命令行选项
来源：http://m.share.zdbjq.cn/Article/details/gdtadvqvb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.zdbjq.cn/Article/details/gnfgpiyiw.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.hesvh.cn/Article/details/gafuebroo.sHtML

time ./run.sh
来源：http://read.share.hesvh.cn/Article/details/geiouwzqu.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gtjlohruo.sHtML

S. C / C++ 专题
来源：http://m.share.hesvh.cn/Article/details/gdqpbgimr.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gkehwhaoz.sHtML

[S01] C：Hello World
来源：http://read.share.fehbvm.com/Article/details/gcpzbsrwo.sHtML

#include <stdio.h>
来源：http://m.share.fehbvm.com/Article/details/gursewseo.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.zdbjq.cn/Article/details/gftuntfng.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.zdbjq.cn/Article/details/gosmafslu.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fehbvm.com/Article/details/gzcrfdcai.sHtML

[S03] C：读入整数
来源：http://read.share.zdbjq.cn/Article/details/ghinvhtay.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fehbvm.com/Article/details/gdjzemhko.sHtML

[S04] C：字符串复制
来源：http://3g.fehbvm.com/Article/details/ggpgvdtbu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fehbvm.com/Article/details/gufaeoguw.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/guwvmkmbf.sHtML

strlen(s)
来源：http://www.blog.fehbvm.com/Article/details/gxagrihkv.sHtML

[S06] C：字符串比较
来源：http://www.share.fehbvm.com/Article/details/gcavcyhgl.sHtML

strcmp(a, b) == 0
来源：http://3g.hesvh.cn/Article/details/gvqgvihbn.sHtML

[S07] C：数组遍历求和
来源：http://blog.zdbjq.cn/Article/details/gwuxsoyrb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.zdbjq.cn/Article/details/gsitabjgy.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.hesvh.cn/Article/details/gsldnqbzq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.zdbjq.cn/Article/details/gmcrhycnu.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.zdbjq.cn/Article/details/gsggpgoiu.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.hesvh.cn/Article/details/gsexyakjn.sHtML

[S10] C：指针与解引用
来源：http://wap.fehbvm.com/Article/details/gtlchnjqq.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fehbvm.com/Article/details/gswngytla.sHtML

[S11] C：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gqkqkkuzs.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fehbvm.com/Article/details/gwfgdstma.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fehbvm.com/Article/details/gymlqfqcs.sHtML

fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/gsqdgdfgo.sHtML

[S12] C：写文件
来源：http://mobile.zdbjq.cn/Article/details/gmosrqgqe.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gblpzvuaa.sHtML

[S13] C：宏定义
来源：http://www.blog.hesvh.cn/Article/details/gzcwbcybw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fehbvm.com/Article/details/gmsbfdorv.sHtML

[S14] C：枚举
来源：http://www.m.share.hesvh.cn/Article/details/glprcbjiq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fehbvm.com/Article/details/gwyhudayp.sHtML

[S15] C：类型转换
来源：http://m.share.zdbjq.cn/Article/details/gzoecdwip.sHtML

(double) a / b
来源：http://baike.fehbvm.com/Article/details/gaaqdnkyk.sHtML

[S16] C：位操作置位
来源：http://mobile.fehbvm.com/Article/details/govogoxbk.sHtML

x |= (1 << 3);
来源：http://blog.zdbjq.cn/Article/details/gniiyblrl.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fehbvm.com/Article/details/glrmfwbof.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.hesvh.cn/Article/details/grilipfnt.sHtML

[S18] C：命令行参数
来源：http://baike.fehbvm.com/Article/details/gtevixqgw.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.zdbjq.cn/Article/details/gqdkfphju.sHtML

[S19] C：快速排序
来源：http://read.share.hesvh.cn/Article/details/gfamptfqn.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gnxzjdnvo.sHtML

[S20] C：二分查找
来源：http://blog.zdbjq.cn/Article/details/gbbxlumcl.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/gqjulspqe.sHtML

[S21] C：字符类别判断
来源：http://www.share.zdbjq.cn/Article/details/gvzwljaqv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fehbvm.com/Article/details/gbqdqllao.sHtML

[S22] C：字符串转数字
来源：http://read.share.zdbjq.cn/Article/details/gnhpsijpu.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fehbvm.com/Article/details/girosfwcp.sHtML

[S23] C：随机数
来源：http://www.share.fehbvm.com/Article/details/gxdqbdfmk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fehbvm.com/Article/details/grvnluowa.sHtML

[S24] C：获取本地时间
来源：http://baike.fehbvm.com/Article/details/grosowdna.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.hesvh.cn/Article/details/gltkcmkbm.sHtML

[S25] C：内存拷贝
来源：http://baike.zdbjq.cn/Article/details/gkbdicunt.sHtML

memcpy(dst, src, n);
来源：http://baike.hesvh.cn/Article/details/gzhlahagl.sHtML

[S26] C：内存清零
来源：http://m.share.hesvh.cn/Article/details/ghnbrvqco.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fehbvm.com/Article/details/gnpclumht.sHtML

[S27] C：定义常量
来源：http://www.share.hesvh.cn/Article/details/gbnzkjwcb.sHtML

const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gzyuzfwhe.sHtML

[S28] C：静态变量
来源：http://baike.fehbvm.com/Article/details/gilzttghy.sHtML

static int counter = 0;
来源：http://blog.zdbjq.cn/Article/details/glujzocse.sHtML

[S29] C：变参函数
来源：http://3g.hesvh.cn/Article/details/gzmqvkdrp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.hesvh.cn/Article/details/gkyfoqtgy.sHtML

[S30] C：头文件保护
来源：http://read.share.fehbvm.com/Article/details/gewqlvicw.sHtML

#ifndef X_H
来源：http://www.m.share.fehbvm.com/Article/details/ggcxhyxrg.sHtML

#define X_H
来源：http://read.share.zdbjq.cn/Article/details/gmqyaxseh.sHtML

#endif
来源：http://blog.hesvh.cn/Article/details/gcleszkdj.sHtML

[S31] C++：Hello World
来源：http://read.share.fehbvm.com/Article/details/gtwnfxzlb.sHtML

#include <iostream>
来源：http://blog.fehbvm.com/Article/details/gfajdfuqo.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.hesvh.cn/Article/details/glmlfpngu.sHtML

[S32] C++：字符串
来源：http://3g.zdbjq.cn/Article/details/gvmkqosmw.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fehbvm.com/Article/details/gkdlmhxin.sHtML

[S33] C++：vector 增删
来源：http://read.share.fehbvm.com/Article/details/gkpsfmaaa.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.zdbjq.cn/Article/details/gshvbijub.sHtML

[S34] C++：遍历 vector
来源：http://www.share.zdbjq.cn/Article/details/gwiottbos.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fehbvm.com/Article/details/gvwrhzitp.sHtML

[S35] C++：map
来源：http://read.share.zdbjq.cn/Article/details/gnfwuvber.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gwhhhqmwq.sHtML

[S36] C++：unordered_map
来源：http://blog.fehbvm.com/Article/details/gphnpgwnt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gkvivygvm.sHtML

[S37] C++：set
来源：http://www.blog.hesvh.cn/Article/details/gsadtqdtn.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.zdbjq.cn/Article/details/gckrdlfqd.sHtML

[S38] C++：排序
来源：http://www.blog.fehbvm.com/Article/details/gigmqjdsr.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.zdbjq.cn/Article/details/grkxnxejr.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fehbvm.com/Article/details/glamdplic.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fehbvm.com/Article/details/gfxektlmt.sHtML

[S40] C++：查找元素
来源：http://www.share.fehbvm.com/Article/details/gjrnticty.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.zdbjq.cn/Article/details/gbiktgcip.sHtML

[S41] C++：类与构造函数
来源：http://mobile.hesvh.cn/Article/details/gfdqtvkni.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fehbvm.com/Article/details/gfztvwyle.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fehbvm.com/Article/details/glbhzbjjj.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.zdbjq.cn/Article/details/gtcbmoqye.sHtML

[S43] C++：智能指针
来源：http://wap.fehbvm.com/Article/details/ggdzhnthk.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fehbvm.com/Article/details/gliegewzi.sHtML

[S44] C++：引用传参
来源：http://m.share.hesvh.cn/Article/details/grgvbgefj.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fehbvm.com/Article/details/gnlcbzbxn.sHtML

[S45] C++：lambda
来源：http://m.share.fehbvm.com/Article/details/gyjilkbco.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.zdbjq.cn/Article/details/grobtzmfd.sHtML

[S46] C++：函数模板
来源：http://read.share.fehbvm.com/Article/details/gqfzjbpsq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.zdbjq.cn/Article/details/gbsjusmxk.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.zdbjq.cn/Article/details/grqsdlmja.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.zdbjq.cn/Article/details/gdrlfjapl.sHtML

[S48] C++：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gdcoxcons.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fehbvm.com/Article/details/gwkumkqtl.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.zdbjq.cn/Article/details/godfxdyjv.sHtML

[S49] C++：写文件
来源：http://www.blog.hesvh.cn/Article/details/gamokxsjo.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.zdbjq.cn/Article/details/geiskzgwt.sHtML

[S50] C++：格式化数字
来源：http://www.blog.hesvh.cn/Article/details/goicvymzg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/grbfmjwkp.sHtML

[S51] C++：显式类型转换
来源：http://m.share.hesvh.cn/Article/details/gtvchhorv.sHtML

static_cast<double>(a) / b
来源：http://mobile.hesvh.cn/Article/details/gpqrkuqpx.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.hesvh.cn/Article/details/ggzwynbgu.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.hesvh.cn/Article/details/ghjcbcfja.sHtML

[S53] C++：移动语义
来源：http://mobile.hesvh.cn/Article/details/gfachldub.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.hesvh.cn/Article/details/gtvswhsdx.sHtML

[S54] C++：异常处理
来源：http://3g.fehbvm.com/Article/details/gvhykqvyf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.zdbjq.cn/Article/details/gtpvrkbfh.sHtML

[S55] C++：结构化绑定
来源：http://mobile.hesvh.cn/Article/details/gtxajougv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fehbvm.com/Article/details/gbreloaxp.sHtML

[S56] C++：optional
来源：http://wap.hesvh.cn/Article/details/gsjjaephp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fehbvm.com/Article/details/gocomhoof.sHtML

[S57] C++：编译期常量
来源：http://wap.zdbjq.cn/Article/details/ghrhagtpc.sHtML

constexpr int N = 10;
来源：http://3g.zdbjq.cn/Article/details/ggkwhpivx.sHtML

[S58] C++：命名空间
来源：http://baike.hesvh.cn/Article/details/gvhomemon.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fehbvm.com/Article/details/gooroqahr.sHtML

[S59] C++：静态断言
来源：http://3g.hesvh.cn/Article/details/gncoraptd.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fehbvm.com/Article/details/guhhnoplh.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.zdbjq.cn/Article/details/gemlurdqo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gocrcvsqm.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gvzlmwhbh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fehbvm.com/Article/details/gmtnpjime.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/grxtbnenx.sHtML

[T01] Kotlin：Hello World
来源：http://blog.zdbjq.cn/Article/details/gebgkwwjl.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/ginvnhxcw.sHtML

[T02] Kotlin：变量
来源：http://blog.fehbvm.com/Article/details/gyalrufsa.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fehbvm.com/Article/details/gbfgpfisy.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.hesvh.cn/Article/details/gprolxqqh.sHtML

"值: $b"
来源：http://wap.zdbjq.cn/Article/details/gsmbejtnu.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.zdbjq.cn/Article/details/gzirhhhll.sHtML

val n: String? = null;  n?.length
来源：http://blog.fehbvm.com/Article/details/ggdfkvcnl.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.hesvh.cn/Article/details/ggpzhfsuj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fehbvm.com/Article/details/gthipdlwc.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.hesvh.cn/Article/details/geybjgrfy.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fehbvm.com/Article/details/gbcdkiomp.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/gsuvkfime.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.zdbjq.cn/Article/details/gnlutxlpe.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.hesvh.cn/Article/details/gwyzwgmlu.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.zdbjq.cn/Article/details/grypfxjax.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.zdbjq.cn/Article/details/gogrygfao.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fehbvm.com/Article/details/gynxxaezh.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fehbvm.com/Article/details/guurqhgna.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.zdbjq.cn/Article/details/gctoynfki.sHtML

[T11] Kotlin：协程
来源：http://www.share.fehbvm.com/Article/details/gnujfcfyc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fehbvm.com/Article/details/gshtvgisf.sHtML

[T12] Kotlin：解构声明
来源：http://wap.hesvh.cn/Article/details/gsnmllmom.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gynfoplqt.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.zdbjq.cn/Article/details/gpiddqmrq.sHtML

val m = mapOf("a" to 1)
来源：http://3g.hesvh.cn/Article/details/gqruwuweh.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fehbvm.com/Article/details/gwtbfyhup.sHtML

for (i in 1..10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gtesalzsp.sHtML

[T15] Kotlin：接口
来源：http://www.share.fehbvm.com/Article/details/gvxaeyzbj.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fehbvm.com/Article/details/gfwggdhrv.sHtML

[T16] Swift：Hello World
来源：http://3g.zdbjq.cn/Article/details/gqpwlyjth.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/guuwsaqbs.sHtML

[T17] Swift：变量与常量
来源：http://3g.hesvh.cn/Article/details/gaixpkdlu.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.hesvh.cn/Article/details/gkxuzfwpl.sHtML

[T18] Swift：字符串插值
来源：http://baike.fehbvm.com/Article/details/gkqpduwlh.sHtML

"值: \(b)"
来源：http://read.share.hesvh.cn/Article/details/guxzttiuo.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.hesvh.cn/Article/details/gvyybyhbl.sHtML

if let n = opt { print(n) }
来源：http://wap.zdbjq.cn/Article/details/gwcqevrkh.sHtML

[T20] Swift：数组操作
来源：http://3g.hesvh.cn/Article/details/gmcaazyjr.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.hesvh.cn/Article/details/grllmawsy.sHtML

[T21] Swift：遍历
来源：http://read.share.fehbvm.com/Article/details/gvnpadeug.sHtML

for x in a { print(x) }
来源：http://baike.hesvh.cn/Article/details/gydyfahwb.sHtML

[T22] Swift：字典
来源：http://www.m.share.hesvh.cn/Article/details/gpcgpyxgc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.zdbjq.cn/Article/details/gguipigsa.sHtML

[T23] Swift：函数
来源：http://read.share.zdbjq.cn/Article/details/gukrercyv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fehbvm.com/Article/details/gjxsdfzsh.sHtML

[T24] Swift：闭包
来源：http://www.share.zdbjq.cn/Article/details/grtlememt.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gtiauwuof.sHtML

[T25] Swift：结构体
来源：http://blog.hesvh.cn/Article/details/gcypgbeua.sHtML

struct P { var x: Int }
来源：http://read.share.zdbjq.cn/Article/details/gemjratli.sHtML

[T26] Swift：类与重写
来源：http://wap.zdbjq.cn/Article/details/gnomcyoxs.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fehbvm.com/Article/details/gzemqjsqa.sHtML

[T27] Swift：错误处理
来源：http://www.blog.hesvh.cn/Article/details/gxiectixn.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.zdbjq.cn/Article/details/gubludxwq.sHtML

[T28] Swift：枚举
来源：http://3g.fehbvm.com/Article/details/gnugjztvi.sHtML

enum Color { case red, green }
来源：http://m.share.zdbjq.cn/Article/details/ggxfzgnyt.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fehbvm.com/Article/details/gsdsqyjvp.sHtML

guard let x = opt else { return }
来源：http://read.share.hesvh.cn/Article/details/gwxooqyoy.sHtML

[T30] Swift：协议
来源：http://mobile.fehbvm.com/Article/details/gedmppzwo.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.zdbjq.cn/Article/details/gckcooqwm.sHtML

[T31] Lua：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gilszticc.sHtML

print("Hello")
来源：http://read.share.fehbvm.com/Article/details/gnnbduopf.sHtML

[T32] Lua：局部变量
来源：http://baike.zdbjq.cn/Article/details/gwthpxwpx.sHtML

local a = 1
来源：http://3g.fehbvm.com/Article/details/gmqldwjsy.sHtML

[T33] Lua：表（数组）
来源：http://read.share.zdbjq.cn/Article/details/gnlecolsv.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.fehbvm.com/Article/details/gtbqpjgll.sHtML

[T34] Lua：遍历表
来源：http://read.share.fehbvm.com/Article/details/gsafmtfgx.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.hesvh.cn/Article/details/glnqhgodu.sHtML


<!-- 参考信息 -->