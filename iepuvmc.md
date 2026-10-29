代发 wailian999

esac
来源：http://mobile.hesvh.cn/Article/details/gyajcbxis.sHtML

[R12] for 遍历文件
来源：http://www.m.share.hesvh.cn/Article/details/gawnfmkzx.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gdqajwxsq.sHtML

[R13] for 计数循环
来源：http://www.share.zdbjq.cn/Article/details/glqqrbtyr.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/guuetyznz.sHtML

[R14] C 风格 for
来源：http://wap.hesvh.cn/Article/details/gllbyfdli.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/guffoandt.sHtML

[R15] while 逐行读文件
来源：http://wap.fehbvm.com/Article/details/gergtrsis.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.hesvh.cn/Article/details/gbyccxpxo.sHtML

[R16] until 等待条件
来源：http://baike.hesvh.cn/Article/details/gkpezxpfq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/gspmldsbc.sHtML

[R17] 数组定义与取值
来源：http://m.share.zdbjq.cn/Article/details/gcwdbtulc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.zdbjq.cn/Article/details/ghmbhriwy.sHtML

[R18] 遍历数组
来源：http://www.blog.fehbvm.com/Article/details/glnduyxjp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.hesvh.cn/Article/details/gkrcojdni.sHtML

[R19] 数组长度
来源：http://read.share.hesvh.cn/Article/details/gkbbvsdwq.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fehbvm.com/Article/details/gqozefoks.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fehbvm.com/Article/details/gruutchdf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fehbvm.com/Article/details/gwhpqpphi.sHtML

[R21] 字符串长度
来源：http://3g.zdbjq.cn/Article/details/gxsscxnsu.sHtML

echo "${#s}"
来源：http://baike.fehbvm.com/Article/details/gndeococr.sHtML

[R22] 截取子串
来源：http://baike.hesvh.cn/Article/details/gdoaxueqq.sHtML

echo "${s:0:5}"
来源：http://www.share.zdbjq.cn/Article/details/gztmdtmal.sHtML

[R23] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/gkydkqdic.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.zdbjq.cn/Article/details/gzxntsztz.sHtML

[R24] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/gmklcmann.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fehbvm.com/Article/details/gonxkxcbx.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fehbvm.com/Article/details/gonlnbdyz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fehbvm.com/Article/details/ggqdyiovu.sHtML

[R26] 命令替换
来源：http://baike.hesvh.cn/Article/details/gahtuugbc.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.zdbjq.cn/Article/details/gwensjyod.sHtML

[R27] 算术展开
来源：http://wap.fehbvm.com/Article/details/gnelfbncq.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.hesvh.cn/Article/details/ghkjhawly.sHtML

[R28] 浮点运算
来源：http://wap.hesvh.cn/Article/details/gistczswl.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fehbvm.com/Article/details/goyiqkedk.sHtML

[R29] 定义函数
来源：http://3g.fehbvm.com/Article/details/gsxpbnhrw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.zdbjq.cn/Article/details/gyxadbrlb.sHtML

[R30] 函数返回状态码
来源：http://baike.hesvh.cn/Article/details/gaeotenlq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.zdbjq.cn/Article/details/gxinulvbu.sHtML

[R31] 局部变量
来源：http://www.blog.hesvh.cn/Article/details/gtnxuormf.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.zdbjq.cn/Article/details/gaylpcmie.sHtML

[R32] 参数个数校验
来源：http://www.m.share.hesvh.cn/Article/details/gpyixwqac.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/gdhppsafv.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.hesvh.cn/Article/details/ggfcailqo.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fehbvm.com/Article/details/gejipdjtm.sHtML

[R34] 退出时清理
来源：http://3g.fehbvm.com/Article/details/gdwudhnnw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/ggrjckczz.sHtML

[R35] 后台执行并等待
来源：http://blog.hesvh.cn/Article/details/genhuidic.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fehbvm.com/Article/details/gnmzenuay.sHtML

[R36] 并发执行多个任务
来源：http://baike.hesvh.cn/Article/details/gypxjkcyl.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fehbvm.com/Article/details/gnmxzijuw.sHtML

[R37] 把输出赋给变量
来源：http://wap.zdbjq.cn/Article/details/gqramorwh.sHtML

files=$(ls -1)
来源：http://m.share.fehbvm.com/Article/details/gffxoztjn.sHtML

[R38] 管道串联
来源：http://baike.hesvh.cn/Article/details/gomwxywfd.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fehbvm.com/Article/details/gmondnfbx.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.hesvh.cn/Article/details/gkilkeavt.sHtML

cmd > out.log 2>&1
来源：http://3g.zdbjq.cn/Article/details/ghimrwfqf.sHtML

[R40] 追加写日志
来源：http://wap.fehbvm.com/Article/details/gcdimzrvx.sHtML

echo "log" >> out.log
来源：http://m.share.hesvh.cn/Article/details/gskycsqlb.sHtML

[R41] 丢弃输出
来源：http://www.blog.hesvh.cn/Article/details/gewdnckis.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.hesvh.cn/Article/details/gausvjyuf.sHtML

[R42] 输入重定向
来源：http://www.share.fehbvm.com/Article/details/gpsflttja.sHtML

wc -l < a.txt
来源：http://www.share.hesvh.cn/Article/details/gllhxtcnc.sHtML

[R43] 按名字查找文件
来源：http://read.share.hesvh.cn/Article/details/gttpznmuj.sHtML

find . -name "*.log" -type f
来源：http://m.share.fehbvm.com/Article/details/gnudpdkfr.sHtML

[R44] 按修改时间查找
来源：http://mobile.zdbjq.cn/Article/details/gwlkplqqc.sHtML

find . -mtime -7 -type f
来源：http://read.share.hesvh.cn/Article/details/gwqaaejam.sHtML

[R45] 批量删除
来源：http://mobile.zdbjq.cn/Article/details/gaafeofzf.sHtML

find . -name "*.tmp" -delete
来源：http://wap.zdbjq.cn/Article/details/gttbvrrug.sHtML

[R46] 递归替换文件内容
来源：http://m.share.zdbjq.cn/Article/details/goojcesjt.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.hesvh.cn/Article/details/gtwpzvhih.sHtML

[R47] sed 单行替换
来源：http://wap.zdbjq.cn/Article/details/gyqfkndbt.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.hesvh.cn/Article/details/grcxgieed.sHtML

[R48] awk 取指定列
来源：http://mobile.zdbjq.cn/Article/details/gdrubffgf.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fehbvm.com/Article/details/gvwtfkbxg.sHtML

[R49] awk 带条件
来源：http://blog.fehbvm.com/Article/details/gwstuwqfy.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.zdbjq.cn/Article/details/gfcpolafy.sHtML

[R50] awk 求和
来源：http://baike.fehbvm.com/Article/details/grfazknid.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gwdvwtefh.sHtML

[R51] 排序去重取前几
来源：http://mobile.hesvh.cn/Article/details/goyrfujpd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fehbvm.com/Article/details/gabmfqpom.sHtML

[R52] 统计行数
来源：http://mobile.hesvh.cn/Article/details/gbnaavfyj.sHtML

wc -l a.txt
来源：http://m.share.hesvh.cn/Article/details/gftzrmkmk.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fehbvm.com/Article/details/gdlmgdrww.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fehbvm.com/Article/details/guxtydtlr.sHtML

[R54] 比较两个文件
来源：http://www.blog.zdbjq.cn/Article/details/gcbwbwhsl.sHtML

diff a.txt b.txt
来源：http://www.blog.hesvh.cn/Article/details/ghfqmaqwo.sHtML

[R55] 压缩与解压
来源：http://m.share.hesvh.cn/Article/details/gbzdlnkbo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.hesvh.cn/Article/details/gwlxfyuhr.sHtML

[R56] 远程拷贝
来源：http://read.share.fehbvm.com/Article/details/gibdyexaa.sHtML

scp file user@host:/path/
来源：http://m.share.hesvh.cn/Article/details/ggqifzueg.sHtML

[R57] 远程执行命令
来源：http://blog.fehbvm.com/Article/details/ghabsankd.sHtML

ssh user@host 'uptime'
来源：http://wap.fehbvm.com/Article/details/goufcuwfc.sHtML

[R58] 下载文件
来源：http://blog.hesvh.cn/Article/details/gmcazqbyr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.hesvh.cn/Article/details/gnkplkhaq.sHtML

[R59] 发 POST JSON
来源：http://3g.zdbjq.cn/Article/details/gtqgtesfu.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fehbvm.com/Article/details/galutucfn.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/gmrrfxmgo.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fehbvm.com/Article/details/gjjqqqnjl.sHtML

[R61] 磁盘占用
来源：http://m.share.hesvh.cn/Article/details/gszikncdc.sHtML

df -h;  du -sh *
来源：http://www.share.zdbjq.cn/Article/details/grmktwiqj.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fehbvm.com/Article/details/gmjkjfbsj.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fehbvm.com/Article/details/gccjudhas.sHtML

[R63] 内存与进程
来源：http://www.m.share.hesvh.cn/Article/details/ggmzxykyy.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.hesvh.cn/Article/details/ghqskaypq.sHtML

[R64] 结束进程
来源：http://www.blog.hesvh.cn/Article/details/glxdhyumz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fehbvm.com/Article/details/gsthokird.sHtML

[R65] 查看端口占用
来源：http://www.blog.fehbvm.com/Article/details/gakheouqj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.hesvh.cn/Article/details/guzlemqfb.sHtML

[R66] 定时任务
来源：http://www.blog.fehbvm.com/Article/details/graszqfls.sHtML

crontab -e;  crontab -l
来源：http://www.share.fehbvm.com/Article/details/guqhmfskw.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fehbvm.com/Article/details/giqlnzmqx.sHtML

openssl rand -hex 16
来源：http://wap.zdbjq.cn/Article/details/gyftdkmsx.sHtML

[R68] 计算文件校验值
来源：http://www.share.hesvh.cn/Article/details/gwhuvvvuh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fehbvm.com/Article/details/ghwbpvhrk.sHtML

[R69] 生成随机密码
来源：http://3g.zdbjq.cn/Article/details/gruynvtyu.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fehbvm.com/Article/details/gwrohixro.sHtML

[R70] 时间戳与互转
来源：http://read.share.zdbjq.cn/Article/details/guybkabxj.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fehbvm.com/Article/details/gkzhbivnx.sHtML

[R71] 日期格式化
来源：http://3g.hesvh.cn/Article/details/ggofjpbnp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fehbvm.com/Article/details/gveboqpwr.sHtML

[R72] 等待端口就绪
来源：http://blog.zdbjq.cn/Article/details/gxrxmwvkv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/gqfjxlfzq.sHtML

[R73] 分割大日志
来源：http://m.share.hesvh.cn/Article/details/giwckgzos.sHtML

split -l 1000 big.log part_
来源：http://blog.hesvh.cn/Article/details/gmmdrbiqv.sHtML

[R74] 批量重命名
来源：http://read.share.zdbjq.cn/Article/details/geniyjalh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.hesvh.cn/Article/details/gvchyirdx.sHtML

[R75] 导出环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gazyjudoq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fehbvm.com/Article/details/giiqwlexq.sHtML

[R76] 使用临时文件
来源：http://m.share.hesvh.cn/Article/details/gmadhcpfo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/gxekzshon.sHtML

[R77] 读取用户输入
来源：http://m.share.hesvh.cn/Article/details/gupkmgxcl.sHtML

read -rp "请输入: " ans
来源：http://wap.fehbvm.com/Article/details/gtplrrgbv.sHtML

[R78] 交互式菜单
来源：http://m.share.hesvh.cn/Article/details/glypdnvpe.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.hesvh.cn/Article/details/gwfhtqmiq.sHtML

[R79] 解析命令行选项
来源：http://m.share.fehbvm.com/Article/details/gjyqavwqw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.zdbjq.cn/Article/details/glgvlfwfs.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fehbvm.com/Article/details/geylmnbbj.sHtML

time ./run.sh
来源：http://blog.fehbvm.com/Article/details/gxvfaohui.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gnehxlrha.sHtML

S. C / C++ 专题
来源：http://read.share.fehbvm.com/Article/details/glyggvkot.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/glaydtchj.sHtML

[S01] C：Hello World
来源：http://wap.hesvh.cn/Article/details/gsdfhdiky.sHtML

#include <stdio.h>
来源：http://read.share.zdbjq.cn/Article/details/ghwaglikx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fehbvm.com/Article/details/ggfpniwoe.sHtML

[S02] C：变量与格式化输出
来源：http://wap.zdbjq.cn/Article/details/gdzhdcffw.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.zdbjq.cn/Article/details/gssgrmjfs.sHtML

[S03] C：读入整数
来源：http://www.share.fehbvm.com/Article/details/gwuaeeiks.sHtML

int x; scanf("%d", &x);
来源：http://blog.hesvh.cn/Article/details/gofdzczdb.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fehbvm.com/Article/details/guuqejsje.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.hesvh.cn/Article/details/giqtkbbhy.sHtML

[S05] C：字符串长度
来源：http://baike.fehbvm.com/Article/details/ghyuqejir.sHtML

strlen(s)
来源：http://3g.fehbvm.com/Article/details/gfmmtzzcy.sHtML

[S06] C：字符串比较
来源：http://3g.zdbjq.cn/Article/details/gcprwqbri.sHtML

strcmp(a, b) == 0
来源：http://baike.fehbvm.com/Article/details/gxpubmkji.sHtML

[S07] C：数组遍历求和
来源：http://m.share.hesvh.cn/Article/details/gybxrnvey.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.zdbjq.cn/Article/details/gnzdezgsp.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.hesvh.cn/Article/details/gxewhqgwg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.zdbjq.cn/Article/details/gcnrgzyqo.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.hesvh.cn/Article/details/gwkectypq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fehbvm.com/Article/details/gvsmqlvbc.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fehbvm.com/Article/details/gbwolcuhw.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.zdbjq.cn/Article/details/gjhrqntci.sHtML

[S11] C：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gdbvpkewr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.zdbjq.cn/Article/details/gmhuvmnul.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fehbvm.com/Article/details/gqjtowihm.sHtML

fclose(f);
来源：http://m.share.hesvh.cn/Article/details/ggkashtnh.sHtML

[S12] C：写文件
来源：http://www.blog.zdbjq.cn/Article/details/ggkqpeoky.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fehbvm.com/Article/details/gbwfeqzro.sHtML

[S13] C：宏定义
来源：http://mobile.hesvh.cn/Article/details/gxufgmuwn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.hesvh.cn/Article/details/gmsubhuji.sHtML

[S14] C：枚举
来源：http://m.share.hesvh.cn/Article/details/gegnosnac.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fehbvm.com/Article/details/gkntiuqui.sHtML

[S15] C：类型转换
来源：http://baike.fehbvm.com/Article/details/gcvcvjmyc.sHtML

(double) a / b
来源：http://www.blog.zdbjq.cn/Article/details/giultounb.sHtML

[S16] C：位操作置位
来源：http://m.share.fehbvm.com/Article/details/gnqcxksrs.sHtML

x |= (1 << 3);
来源：http://wap.zdbjq.cn/Article/details/ghlvyrtoo.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gxvdndist.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.zdbjq.cn/Article/details/gddahvvsm.sHtML

[S18] C：命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/guhbfitul.sHtML

int main(int argc, char **argv)
来源：http://3g.zdbjq.cn/Article/details/gazcbjnqz.sHtML

[S19] C：快速排序
来源：http://read.share.zdbjq.cn/Article/details/gyfforovv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/glbntqzni.sHtML

[S20] C：二分查找
来源：http://3g.hesvh.cn/Article/details/gggxetiwe.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gxyvhzbsg.sHtML

[S21] C：字符类别判断
来源：http://wap.zdbjq.cn/Article/details/gdgwgzkyk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.hesvh.cn/Article/details/gdfbekiuq.sHtML

[S22] C：字符串转数字
来源：http://wap.zdbjq.cn/Article/details/gqvhxjtgd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.hesvh.cn/Article/details/gckchgkiu.sHtML

[S23] C：随机数
来源：http://www.share.fehbvm.com/Article/details/gxnkjofrf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.zdbjq.cn/Article/details/grclsfsbr.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.hesvh.cn/Article/details/gzzxdikzp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.zdbjq.cn/Article/details/gdjuwxseg.sHtML

[S25] C：内存拷贝
来源：http://mobile.zdbjq.cn/Article/details/gsugwsbjh.sHtML

memcpy(dst, src, n);
来源：http://mobile.zdbjq.cn/Article/details/gereshyri.sHtML

[S26] C：内存清零
来源：http://3g.fehbvm.com/Article/details/gbujbymtu.sHtML

memset(a, 0, sizeof a);
来源：http://wap.zdbjq.cn/Article/details/gaizudjtk.sHtML

[S27] C：定义常量
来源：http://3g.zdbjq.cn/Article/details/gczgfeumv.sHtML

const double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/guxcxugsx.sHtML

[S28] C：静态变量
来源：http://www.blog.hesvh.cn/Article/details/gsntgulgb.sHtML

static int counter = 0;
来源：http://www.m.share.hesvh.cn/Article/details/gfqqrzyxs.sHtML

[S29] C：变参函数
来源：http://read.share.zdbjq.cn/Article/details/gqhxywtli.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fehbvm.com/Article/details/gdmyxewos.sHtML

[S30] C：头文件保护
来源：http://m.share.hesvh.cn/Article/details/gnemtaeiv.sHtML

#ifndef X_H
来源：http://mobile.fehbvm.com/Article/details/gqndkiyin.sHtML

#define X_H
来源：http://baike.hesvh.cn/Article/details/gfphuitgp.sHtML

#endif
来源：http://3g.hesvh.cn/Article/details/gkcevuuvm.sHtML

[S31] C++：Hello World
来源：http://baike.fehbvm.com/Article/details/gjuomvdpv.sHtML

#include <iostream>
来源：http://www.m.share.zdbjq.cn/Article/details/gyvdxwnyo.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fehbvm.com/Article/details/gfngcksps.sHtML

[S32] C++：字符串
来源：http://www.blog.zdbjq.cn/Article/details/gtfotkzpr.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fehbvm.com/Article/details/gmpqzzsar.sHtML

[S33] C++：vector 增删
来源：http://read.share.hesvh.cn/Article/details/gpoibnhmb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.zdbjq.cn/Article/details/ggsdusuni.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fehbvm.com/Article/details/gnnonlflp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.hesvh.cn/Article/details/gyzvsaxfb.sHtML

[S35] C++：map
来源：http://blog.hesvh.cn/Article/details/gfwgwvefc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/gmykitilk.sHtML

[S36] C++：unordered_map
来源：http://baike.zdbjq.cn/Article/details/gkmnrulzt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gqkijohfp.sHtML

[S37] C++：set
来源：http://mobile.zdbjq.cn/Article/details/gmovgmvhv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.zdbjq.cn/Article/details/gutzytyyz.sHtML

[S38] C++：排序
来源：http://www.blog.hesvh.cn/Article/details/gigroggrv.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.hesvh.cn/Article/details/ggvatbpba.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.zdbjq.cn/Article/details/gmrpayhlu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.zdbjq.cn/Article/details/gikxnkhen.sHtML

[S40] C++：查找元素
来源：http://3g.fehbvm.com/Article/details/gkdjlpmcx.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.hesvh.cn/Article/details/gyupepgof.sHtML

[S41] C++：类与构造函数
来源：http://baike.hesvh.cn/Article/details/gxkipscdh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.hesvh.cn/Article/details/gqjsiyrca.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fehbvm.com/Article/details/gtwdqfgie.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.zdbjq.cn/Article/details/ggqmjserr.sHtML

[S43] C++：智能指针
来源：http://www.blog.hesvh.cn/Article/details/gkoutekhs.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.hesvh.cn/Article/details/gcgvcrjpo.sHtML

[S44] C++：引用传参
来源：http://baike.zdbjq.cn/Article/details/gmkejvhxz.sHtML

void inc(int &x) { ++x; }
来源：http://3g.hesvh.cn/Article/details/gjqnacoke.sHtML

[S45] C++：lambda
来源：http://3g.zdbjq.cn/Article/details/gfztftvsm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fehbvm.com/Article/details/gehsmnptq.sHtML

[S46] C++：函数模板
来源：http://read.share.hesvh.cn/Article/details/gtaufmlxi.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fehbvm.com/Article/details/ghnnpmycd.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fehbvm.com/Article/details/geafwpucw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.hesvh.cn/Article/details/ggocbkmiq.sHtML

[S48] C++：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gtqfarazs.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.zdbjq.cn/Article/details/gxhfnxasa.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fehbvm.com/Article/details/gyjffhygp.sHtML

[S49] C++：写文件
来源：http://mobile.zdbjq.cn/Article/details/gdwcthovy.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fehbvm.com/Article/details/gnuqdtstx.sHtML

[S50] C++：格式化数字
来源：http://www.blog.hesvh.cn/Article/details/gvypfkzur.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gsimlbqlz.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.zdbjq.cn/Article/details/gpxxivslm.sHtML

static_cast<double>(a) / b
来源：http://wap.zdbjq.cn/Article/details/gzaeladif.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fehbvm.com/Article/details/gsxtcrnar.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsirovyaa.sHtML

[S53] C++：移动语义
来源：http://blog.fehbvm.com/Article/details/gocydtokm.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.hesvh.cn/Article/details/ghhpfxnip.sHtML

[S54] C++：异常处理
来源：http://www.share.hesvh.cn/Article/details/gcresdiae.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fehbvm.com/Article/details/gpqwbjcty.sHtML

[S55] C++：结构化绑定
来源：http://blog.fehbvm.com/Article/details/gwsazaiqr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.hesvh.cn/Article/details/gshomxmzh.sHtML

[S56] C++：optional
来源：http://www.blog.fehbvm.com/Article/details/gbfxkvfaw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fehbvm.com/Article/details/gnylkiaal.sHtML

[S57] C++：编译期常量
来源：http://www.share.fehbvm.com/Article/details/gzhvycbmo.sHtML

constexpr int N = 10;
来源：http://3g.hesvh.cn/Article/details/gptyjdpbe.sHtML

[S58] C++：命名空间
来源：http://wap.fehbvm.com/Article/details/gquethmxf.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.hesvh.cn/Article/details/ggkhdiayt.sHtML

[S59] C++：静态断言
来源：http://mobile.fehbvm.com/Article/details/gjnlrzcwg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.hesvh.cn/Article/details/gonrigwva.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.zdbjq.cn/Article/details/gnowxedov.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.zdbjq.cn/Article/details/grsykxxcc.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gcixsedeu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.zdbjq.cn/Article/details/gmalrvgpf.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/glbqmunae.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fehbvm.com/Article/details/gckjzazkn.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/gykcpvzwz.sHtML

[T02] Kotlin：变量
来源：http://3g.hesvh.cn/Article/details/gbruxgprc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fehbvm.com/Article/details/gyldvgzqa.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.zdbjq.cn/Article/details/glzivgoex.sHtML

"值: $b"
来源：http://baike.fehbvm.com/Article/details/gmxadbags.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fehbvm.com/Article/details/gefewpmqa.sHtML

val n: String? = null;  n?.length
来源：http://m.share.zdbjq.cn/Article/details/ghastgpeo.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.hesvh.cn/Article/details/gstodphuj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fehbvm.com/Article/details/gogrrpmkm.sHtML

[T06] Kotlin：集合映射
来源：http://baike.zdbjq.cn/Article/details/gvsanutyz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.zdbjq.cn/Article/details/gdbljrpmw.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/guzyzhrit.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.hesvh.cn/Article/details/gckknwivo.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.zdbjq.cn/Article/details/glztnnroc.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.hesvh.cn/Article/details/gmxvhegam.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fehbvm.com/Article/details/gomcccvwz.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.hesvh.cn/Article/details/gnosvvwcz.sHtML

[T10] Kotlin：默认参数
来源：http://baike.zdbjq.cn/Article/details/gndxxcajr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.zdbjq.cn/Article/details/ggkhpwioy.sHtML

[T11] Kotlin：协程
来源：http://baike.hesvh.cn/Article/details/guvlbxjlm.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fehbvm.com/Article/details/guspcupik.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fehbvm.com/Article/details/gulxwadwx.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gwumecynl.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fehbvm.com/Article/details/gerkvlnqi.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fehbvm.com/Article/details/grtqvexad.sHtML

[T14] Kotlin：循环
来源：http://blog.zdbjq.cn/Article/details/gnrsinjqb.sHtML

for (i in 1..10) println(i)
来源：http://m.share.hesvh.cn/Article/details/gjssyuqwc.sHtML


<!-- 参考信息 -->