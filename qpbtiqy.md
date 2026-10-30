代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggwnnlzbi.sHtML

[R32] 参数个数校验
来源：http://wap.fanxiaobao.xyz/Article/details/ghyngqrbn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqqykcmuu.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gulstruwh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fanxiaobao.xyz/Article/details/gtponqjsw.sHtML

[R34] 退出时清理
来源：http://m.share.fanxiaobao.xyz/Article/details/gqvfxdwas.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqrjchrjt.sHtML

[R35] 后台执行并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/glnsdkawa.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fanxiaobao.xyz/Article/details/glcuidcln.sHtML

[R36] 并发执行多个任务
来源：http://baike.fanxiaobao.xyz/Article/details/gthkmmwtt.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fanxiaobao.xyz/Article/details/gynqoxvji.sHtML

[R37] 把输出赋给变量
来源：http://3g.fanxiaobao.xyz/Article/details/gipvfceau.sHtML

files=$(ls -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gaoijorlm.sHtML

[R38] 管道串联
来源：http://3g.fanxiaobao.xyz/Article/details/gnoiqhtec.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gncrrdesz.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fanxiaobao.xyz/Article/details/ghorkrrlu.sHtML

cmd > out.log 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/ghiksomvb.sHtML

[R40] 追加写日志
来源：http://baike.fanxiaobao.xyz/Article/details/glzqnxtid.sHtML

echo "log" >> out.log
来源：http://blog.fanxiaobao.xyz/Article/details/gkaadvjhi.sHtML

[R41] 丢弃输出
来源：http://mobile.fanxiaobao.xyz/Article/details/golnmupov.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gztkmcbxc.sHtML

[R42] 输入重定向
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqtoqumc.sHtML

wc -l < a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gztqngbyx.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/giancempf.sHtML

find . -name "*.log" -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/glpxfgeai.sHtML

[R44] 按修改时间查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gdyltgaql.sHtML

find . -mtime -7 -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gmzxiupuw.sHtML

[R45] 批量删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gntuadwnx.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fanxiaobao.xyz/Article/details/gkldeumxs.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/gxgbtudhq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fanxiaobao.xyz/Article/details/gaslvukwn.sHtML

[R47] sed 单行替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkiiaarp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gftfnrxzy.sHtML

[R48] awk 取指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqnaddaub.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/ghwmvfzuk.sHtML

[R49] awk 带条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gsylvnuig.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fanxiaobao.xyz/Article/details/gdvihdvjw.sHtML

[R50] awk 求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gparohkjh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gximalckm.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdtfjvlvk.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fanxiaobao.xyz/Article/details/gujugfnyb.sHtML

[R52] 统计行数
来源：http://3g.fanxiaobao.xyz/Article/details/geckvrrac.sHtML

wc -l a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/glewxqhxd.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmoczihbx.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fanxiaobao.xyz/Article/details/gifsgyfzo.sHtML

[R54] 比较两个文件
来源：http://baike.fanxiaobao.xyz/Article/details/gqvhlwosa.sHtML

diff a.txt b.txt
来源：http://baike.fanxiaobao.xyz/Article/details/goiaoyrvn.sHtML

[R55] 压缩与解压
来源：http://mobile.fanxiaobao.xyz/Article/details/geqyassvz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjhwkzui.sHtML

[R56] 远程拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjzrazsw.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/ggkdevwok.sHtML

[R57] 远程执行命令
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpkqlpngu.sHtML

ssh user@host 'uptime'
来源：http://m.share.fanxiaobao.xyz/Article/details/gfcmpccgb.sHtML

[R58] 下载文件
来源：http://wap.fanxiaobao.xyz/Article/details/gtrexhirx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/gmpllevmb.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpedenpzp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fanxiaobao.xyz/Article/details/gzenqnvcu.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gyucwjnce.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fanxiaobao.xyz/Article/details/glawbxlxi.sHtML

[R61] 磁盘占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gficzddei.sHtML

df -h;  du -sh *
来源：http://m.share.fanxiaobao.xyz/Article/details/glimlpyur.sHtML

[R62] 找最占空间的文件
来源：http://baike.fanxiaobao.xyz/Article/details/gdstodlip.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fanxiaobao.xyz/Article/details/gdinmbjoz.sHtML

[R63] 内存与进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gwsrsgrvx.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fanxiaobao.xyz/Article/details/gwgzzjcyi.sHtML

[R64] 结束进程
来源：http://blog.fanxiaobao.xyz/Article/details/gylgjtbax.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghcbvmgwx.sHtML

[R65] 查看端口占用
来源：http://baike.fanxiaobao.xyz/Article/details/gehwltona.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzcrysvte.sHtML

[R66] 定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/guddpitso.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyarvsfdd.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fanxiaobao.xyz/Article/details/gmmgtnvwm.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/grfifemky.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnlgnvgll.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gxcnrnivn.sHtML

[R69] 生成随机密码
来源：http://read.share.fanxiaobao.xyz/Article/details/gbtghrqxe.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fanxiaobao.xyz/Article/details/gaxaeskgo.sHtML

[R70] 时间戳与互转
来源：http://www.share.fanxiaobao.xyz/Article/details/gizardusc.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fanxiaobao.xyz/Article/details/gnwfgknlp.sHtML

[R71] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gyuzzuual.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fanxiaobao.xyz/Article/details/ggghurvfo.sHtML

[R72] 等待端口就绪
来源：http://baike.fanxiaobao.xyz/Article/details/gqueqvfwo.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyszcjrda.sHtML

[R73] 分割大日志
来源：http://baike.fanxiaobao.xyz/Article/details/gtjdqjymz.sHtML

split -l 1000 big.log part_
来源：http://read.share.fanxiaobao.xyz/Article/details/ghgcrhful.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtsnbppdk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/grzpizsxc.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzvqmbipk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/gyttwiirj.sHtML

[R76] 使用临时文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gkczdjbot.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbqxmjxuf.sHtML

[R77] 读取用户输入
来源：http://wap.fanxiaobao.xyz/Article/details/gfowrqbmf.sHtML

read -rp "请输入: " ans
来源：http://read.share.fanxiaobao.xyz/Article/details/gihogcmjx.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guuqtirvi.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjvnnlagp.sHtML

[R79] 解析命令行选项
来源：http://wap.fanxiaobao.xyz/Article/details/gqcznyvmj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gdulvupfq.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggtrloqub.sHtML

time ./run.sh
来源：http://m.share.fanxiaobao.xyz/Article/details/ghxelplfr.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gdsqboxxd.sHtML

S. C / C++ 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gupiznwro.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gpdvidjzt.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gyzpkneks.sHtML

#include <stdio.h>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnhitmvmd.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggmjsflin.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gettybwhi.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fanxiaobao.xyz/Article/details/gkwmrkrnh.sHtML

[S03] C：读入整数
来源：http://blog.fanxiaobao.xyz/Article/details/gchnacgwl.sHtML

int x; scanf("%d", &x);
来源：http://blog.fanxiaobao.xyz/Article/details/gonjgsoll.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/gduvxmicp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/gfowwwvbj.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gnejewaty.sHtML

strlen(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqjqblypn.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gjccfndak.sHtML

strcmp(a, b) == 0
来源：http://read.share.fanxiaobao.xyz/Article/details/gyfhtvddb.sHtML

[S07] C：数组遍历求和
来源：http://wap.fanxiaobao.xyz/Article/details/gsdtlpykb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gktztbbam.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fanxiaobao.xyz/Article/details/gfhdzwbpq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grlqyzwin.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fanxiaobao.xyz/Article/details/gnpxpxfxc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fanxiaobao.xyz/Article/details/gkaynqzlt.sHtML

[S10] C：指针与解引用
来源：http://read.share.fanxiaobao.xyz/Article/details/gfsrbddpr.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fanxiaobao.xyz/Article/details/gfvotowln.sHtML

[S11] C：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/grmxakzie.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/geglxvpvq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/ggembyhhz.sHtML

fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/ggzvgyydi.sHtML

[S12] C：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gqjotqbkm.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glnaadlbu.sHtML

[S13] C：宏定义
来源：http://blog.fanxiaobao.xyz/Article/details/goewlqwso.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fanxiaobao.xyz/Article/details/gvvwjylwb.sHtML

[S14] C：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxraaguby.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdztomdep.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdgowvkom.sHtML

(double) a / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gggsdysdj.sHtML

[S16] C：位操作置位
来源：http://read.share.fanxiaobao.xyz/Article/details/gqyoijfgp.sHtML

x |= (1 << 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gridqozkv.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/ghpobynbw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fanxiaobao.xyz/Article/details/ghkcsgohb.sHtML

[S18] C：命令行参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gozvqsevx.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggxggrhrn.sHtML

[S19] C：快速排序
来源：http://baike.fanxiaobao.xyz/Article/details/gjlrtrcol.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxzjlpwy.sHtML

[S20] C：二分查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gykkbnvgk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmukfijxo.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gpgivsryf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fanxiaobao.xyz/Article/details/glzwljhxv.sHtML

[S22] C：字符串转数字
来源：http://baike.fanxiaobao.xyz/Article/details/gmikecclg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkeyjggef.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/gqgmfgeus.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkkmtgmua.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/gqlfktlrg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fanxiaobao.xyz/Article/details/gyaspdbru.sHtML

[S25] C：内存拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gemcfuxrm.sHtML

memcpy(dst, src, n);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjdpdtjrl.sHtML

[S26] C：内存清零
来源：http://wap.fanxiaobao.xyz/Article/details/gjamilihc.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fanxiaobao.xyz/Article/details/gvghlkvqd.sHtML

[S27] C：定义常量
来源：http://baike.fanxiaobao.xyz/Article/details/gayxkruxw.sHtML

const double PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdpqrwpmk.sHtML

[S28] C：静态变量
来源：http://wap.fanxiaobao.xyz/Article/details/ggblreljv.sHtML

static int counter = 0;
来源：http://baike.fanxiaobao.xyz/Article/details/gzadekfti.sHtML

[S29] C：变参函数
来源：http://3g.fanxiaobao.xyz/Article/details/gqiaqczra.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gitkddyzx.sHtML

[S30] C：头文件保护
来源：http://3g.fanxiaobao.xyz/Article/details/gjlcdfbyd.sHtML

#ifndef X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geuoxldrf.sHtML

#define X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gdxfkezml.sHtML

#endif
来源：http://mobile.fanxiaobao.xyz/Article/details/gxoxbcsmz.sHtML

[S31] C++：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gfkttoojq.sHtML

#include <iostream>
来源：http://blog.fanxiaobao.xyz/Article/details/geuxhqqtj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gayahmror.sHtML

[S32] C++：字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gtmmuacxo.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fanxiaobao.xyz/Article/details/glkrrlngz.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmogfofrk.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdsiohmvj.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fanxiaobao.xyz/Article/details/gbcqbuhkl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gpzcmjglj.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/grxkuhhdr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gkhdgnlna.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxlgykax.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gahrjdikx.sHtML

[S37] C++：set
来源：http://3g.fanxiaobao.xyz/Article/details/ggrojypuw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gaykqehoc.sHtML

[S38] C++：排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnlvtnind.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/grmdrajod.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gxhlhpeoq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxvuvycj.sHtML

[S40] C++：查找元素
来源：http://wap.fanxiaobao.xyz/Article/details/gcsillehv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gehlfauaf.sHtML

[S41] C++：类与构造函数
来源：http://baike.fanxiaobao.xyz/Article/details/gayfunpxa.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fanxiaobao.xyz/Article/details/gcvjuldbj.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gtdstwshs.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fanxiaobao.xyz/Article/details/ggckjgobv.sHtML

[S43] C++：智能指针
来源：http://3g.fanxiaobao.xyz/Article/details/grmettlln.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdfqocrvu.sHtML

[S44] C++：引用传参
来源：http://wap.fanxiaobao.xyz/Article/details/gswifpett.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gzaavlzuv.sHtML

[S45] C++：lambda
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gigeccnai.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gfcobngee.sHtML

[S46] C++：函数模板
来源：http://wap.fanxiaobao.xyz/Article/details/gqcriaxsz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqubfwmfn.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gvuyvhofu.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fanxiaobao.xyz/Article/details/gmnzebpne.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gbmcvuych.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnyfqipbd.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxsanbxo.sHtML

[S49] C++：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/giknuxpul.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvnzqsxb.sHtML

[S50] C++：格式化数字
来源：http://3g.fanxiaobao.xyz/Article/details/gjsbnnegv.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gtmfmzldg.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gorbuipqx.sHtML

static_cast<double>(a) / b
来源：http://wap.fanxiaobao.xyz/Article/details/gadhmrrgh.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fanxiaobao.xyz/Article/details/gepeliruh.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxokrieg.sHtML

[S53] C++：移动语义
来源：http://mobile.fanxiaobao.xyz/Article/details/gkouxyxqw.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fanxiaobao.xyz/Article/details/gibgampve.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijhsmlst.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gekvghvns.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gfzjzdzho.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gpzbqfgae.sHtML

[S56] C++：optional
来源：http://baike.fanxiaobao.xyz/Article/details/gjdwsdnou.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzusazeid.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdoitpprs.sHtML

constexpr int N = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gxtrvbbdt.sHtML

[S58] C++：命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/glmbomshj.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsmzygejm.sHtML

[S59] C++：静态断言
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbpkxavr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fanxiaobao.xyz/Article/details/gmrnfppxd.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fanxiaobao.xyz/Article/details/gstzyjovn.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gchdubtms.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvhasgnb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fanxiaobao.xyz/Article/details/gqdyyqsim.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/ggxibbqrs.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcjadlwvt.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gtocokvxp.sHtML

[T02] Kotlin：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gpgxuiliy.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwrbqaya.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gzkhxboir.sHtML

"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/gagrlwquu.sHtML

[T04] Kotlin：空安全
来源：http://wap.fanxiaobao.xyz/Article/details/gqrecdmrt.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gdfmsuheg.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzcwfmkhw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fanxiaobao.xyz/Article/details/gzbqhsldy.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejaibbsq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxnocrgxo.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gxtkmnutz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfpdfblbm.sHtML

[T08] Kotlin：数据类
来源：http://blog.fanxiaobao.xyz/Article/details/gziroywur.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fanxiaobao.xyz/Article/details/gddzfomij.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gdyvfyccq.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fanxiaobao.xyz/Article/details/gekbekiwp.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gnlziphrh.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxnbogesu.sHtML

[T11] Kotlin：协程
来源：http://m.share.fanxiaobao.xyz/Article/details/gcfsrhbbl.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fanxiaobao.xyz/Article/details/giijnmmmg.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fanxiaobao.xyz/Article/details/gfmbyxaxo.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/grsfleiwp.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fanxiaobao.xyz/Article/details/gugrkglxd.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gdktxhxoi.sHtML

[T14] Kotlin：循环
来源：http://blog.fanxiaobao.xyz/Article/details/gziaqiqfe.sHtML

for (i in 1..10) println(i)
来源：http://wap.fanxiaobao.xyz/Article/details/gdjyfngfu.sHtML

[T15] Kotlin：接口
来源：http://blog.fanxiaobao.xyz/Article/details/gfcbtbogb.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fanxiaobao.xyz/Article/details/goizsdycy.sHtML

[T16] Swift：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gpeiklfpb.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnrlclvjx.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gifmmsfmo.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtppxeaaz.sHtML

[T18] Swift：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gbvkqsnuu.sHtML

"值: \(b)"
来源：http://baike.fanxiaobao.xyz/Article/details/gyndtgvnu.sHtML

[T19] Swift：可选绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gsffulpmg.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwljtazfw.sHtML

[T20] Swift：数组操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gmukntpvb.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fanxiaobao.xyz/Article/details/gkziwjpbv.sHtML

[T21] Swift：遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gjtsmyetw.sHtML

for x in a { print(x) }
来源：http://wap.fanxiaobao.xyz/Article/details/gfubnvvzo.sHtML

[T22] Swift：字典
来源：http://blog.fanxiaobao.xyz/Article/details/gjcbdkmar.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gnyueguae.sHtML

[T23] Swift：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gpclfgfuo.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzmlmvyvm.sHtML

[T24] Swift：闭包
来源：http://wap.fanxiaobao.xyz/Article/details/ggqlowaib.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpejmglsg.sHtML

[T25] Swift：结构体
来源：http://baike.fanxiaobao.xyz/Article/details/gqvigfwjt.sHtML

struct P { var x: Int }
来源：http://blog.fanxiaobao.xyz/Article/details/glopymkhq.sHtML

[T26] Swift：类与重写
来源：http://read.share.fanxiaobao.xyz/Article/details/glmhmcare.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozvhoebr.sHtML

[T27] Swift：错误处理
来源：http://mobile.fanxiaobao.xyz/Article/details/grbcqxfqf.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxheatkck.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvpjdmsfc.sHtML

enum Color { case red, green }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggvsqlnoq.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyctmipdt.sHtML

guard let x = opt else { return }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvinvpfk.sHtML

[T30] Swift：协议
来源：http://mobile.fanxiaobao.xyz/Article/details/gypayjxzy.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fanxiaobao.xyz/Article/details/gopqdpbtk.sHtML

[T31] Lua：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gtfhdnkng.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gvckjahil.sHtML

[T32] Lua：局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gptqhmrze.sHtML

local a = 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjobpsmo.sHtML

[T33] Lua：表（数组）
来源：http://3g.fanxiaobao.xyz/Article/details/gvqmmqyvy.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.fanxiaobao.xyz/Article/details/glpozgsme.sHtML

[T34] Lua：遍历表
来源：http://3g.fanxiaobao.xyz/Article/details/gkybzjrgz.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fanxiaobao.xyz/Article/details/gtxsadnrx.sHtML


<!-- 参考信息 -->