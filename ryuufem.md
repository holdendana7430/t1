代发 wailian999

esac
来源：http://m.share.fehbvm.com/Article/details/gzlihpmkk.sHtML

[R12] for 遍历文件
来源：http://read.share.zdbjq.cn/Article/details/gfrzeenmz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.zdbjq.cn/Article/details/gawoshgpl.sHtML

[R13] for 计数循环
来源：http://www.blog.fehbvm.com/Article/details/gjnzcvzpw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/gnjnuwlgg.sHtML

[R14] C 风格 for
来源：http://read.share.zdbjq.cn/Article/details/gvwmilmhp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/gxfxdopgz.sHtML

[R15] while 逐行读文件
来源：http://www.share.hesvh.cn/Article/details/ganggoqoj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.hesvh.cn/Article/details/gfebitmpm.sHtML

[R16] until 等待条件
来源：http://www.m.share.fehbvm.com/Article/details/gptunjmtq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/goqcxmrwu.sHtML

[R17] 数组定义与取值
来源：http://read.share.fehbvm.com/Article/details/gcmzndoom.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.hesvh.cn/Article/details/gtgnomixe.sHtML

[R18] 遍历数组
来源：http://mobile.zdbjq.cn/Article/details/gifvssjtr.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.hesvh.cn/Article/details/geptxtjay.sHtML

[R19] 数组长度
来源：http://mobile.hesvh.cn/Article/details/gsxujcrtv.sHtML

echo "${#arr[@]}"
来源：http://mobile.zdbjq.cn/Article/details/gjkkkqtzf.sHtML

[R20] 关联数组（字典）
来源：http://3g.hesvh.cn/Article/details/genyhoasw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.zdbjq.cn/Article/details/gdpfvhbiw.sHtML

[R21] 字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/gdgjqbciv.sHtML

echo "${#s}"
来源：http://baike.hesvh.cn/Article/details/gaekkrcvt.sHtML

[R22] 截取子串
来源：http://read.share.fehbvm.com/Article/details/gyhqbcnnv.sHtML

echo "${s:0:5}"
来源：http://www.blog.hesvh.cn/Article/details/guquuazjt.sHtML

[R23] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gkawrkxem.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.zdbjq.cn/Article/details/gpauztdyx.sHtML

[R24] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/ghcpbbwan.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fehbvm.com/Article/details/gxmhpxldg.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fehbvm.com/Article/details/gfkhzuzgh.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.hesvh.cn/Article/details/gzpcybhtx.sHtML

[R26] 命令替换
来源：http://mobile.hesvh.cn/Article/details/gbdbpizpf.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fehbvm.com/Article/details/gstcoxgfm.sHtML

[R27] 算术展开
来源：http://wap.zdbjq.cn/Article/details/grdjkhmej.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.hesvh.cn/Article/details/gptqauyys.sHtML

[R28] 浮点运算
来源：http://wap.fehbvm.com/Article/details/gcypaqcxc.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.hesvh.cn/Article/details/gcvekwrva.sHtML

[R29] 定义函数
来源：http://mobile.fehbvm.com/Article/details/gsktcifau.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.hesvh.cn/Article/details/gmxyqsial.sHtML

[R30] 函数返回状态码
来源：http://wap.fehbvm.com/Article/details/gcvxvlwpk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fehbvm.com/Article/details/goejykbeg.sHtML

[R31] 局部变量
来源：http://baike.zdbjq.cn/Article/details/gvalhpwir.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.hesvh.cn/Article/details/gpjqpippb.sHtML

[R32] 参数个数校验
来源：http://mobile.zdbjq.cn/Article/details/glbognofr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/gnmedckqo.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.zdbjq.cn/Article/details/gkwomnivu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fehbvm.com/Article/details/gzvrhyish.sHtML

[R34] 退出时清理
来源：http://baike.zdbjq.cn/Article/details/glqtsbkca.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/grakzfjff.sHtML

[R35] 后台执行并等待
来源：http://blog.hesvh.cn/Article/details/gcaobreuw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fehbvm.com/Article/details/gwvxwiada.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fehbvm.com/Article/details/gwdzezvwr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.zdbjq.cn/Article/details/gygcepygv.sHtML

[R37] 把输出赋给变量
来源：http://blog.zdbjq.cn/Article/details/gamdhjtej.sHtML

files=$(ls -1)
来源：http://www.share.zdbjq.cn/Article/details/gjszmzpis.sHtML

[R38] 管道串联
来源：http://read.share.fehbvm.com/Article/details/gmlvesutb.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.hesvh.cn/Article/details/gkuxshman.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.hesvh.cn/Article/details/gftzhfxjh.sHtML

cmd > out.log 2>&1
来源：http://mobile.zdbjq.cn/Article/details/gzhofqytr.sHtML

[R40] 追加写日志
来源：http://mobile.zdbjq.cn/Article/details/gkkiomgvq.sHtML

echo "log" >> out.log
来源：http://baike.hesvh.cn/Article/details/gstxzsuep.sHtML

[R41] 丢弃输出
来源：http://3g.fehbvm.com/Article/details/gbpmqxghc.sHtML

cmd >/dev/null 2>&1
来源：http://blog.zdbjq.cn/Article/details/gurjazjem.sHtML

[R42] 输入重定向
来源：http://www.m.share.fehbvm.com/Article/details/girqgsvwh.sHtML

wc -l < a.txt
来源：http://www.blog.hesvh.cn/Article/details/ggptlmdwa.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fehbvm.com/Article/details/gwcuutlnf.sHtML

find . -name "*.log" -type f
来源：http://3g.hesvh.cn/Article/details/ggloazotb.sHtML

[R44] 按修改时间查找
来源：http://read.share.hesvh.cn/Article/details/gyuabrozb.sHtML

find . -mtime -7 -type f
来源：http://read.share.hesvh.cn/Article/details/gkqqsuxrk.sHtML

[R45] 批量删除
来源：http://www.share.hesvh.cn/Article/details/gkhorgdih.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fehbvm.com/Article/details/ghxfzbngr.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.zdbjq.cn/Article/details/gajtlaxqa.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fehbvm.com/Article/details/glfjmiiow.sHtML

[R47] sed 单行替换
来源：http://m.share.hesvh.cn/Article/details/ghubvuehd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fehbvm.com/Article/details/gesjacqmi.sHtML

[R48] awk 取指定列
来源：http://www.blog.fehbvm.com/Article/details/gofpaboxe.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fehbvm.com/Article/details/gfstluiqr.sHtML

[R49] awk 带条件
来源：http://www.blog.hesvh.cn/Article/details/ghgclovmv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.hesvh.cn/Article/details/gizvqoydz.sHtML

[R50] awk 求和
来源：http://wap.fehbvm.com/Article/details/gsgserbkh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.zdbjq.cn/Article/details/gtpsdsrhl.sHtML

[R51] 排序去重取前几
来源：http://www.share.hesvh.cn/Article/details/geqochise.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.hesvh.cn/Article/details/gkkufyxqc.sHtML

[R52] 统计行数
来源：http://blog.zdbjq.cn/Article/details/gejwzhjna.sHtML

wc -l a.txt
来源：http://baike.fehbvm.com/Article/details/gsjgxkuwq.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.zdbjq.cn/Article/details/gqdjgybkz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.hesvh.cn/Article/details/gwihadhwo.sHtML

[R54] 比较两个文件
来源：http://blog.fehbvm.com/Article/details/gnvpildoq.sHtML

diff a.txt b.txt
来源：http://www.m.share.fehbvm.com/Article/details/gmfjelrda.sHtML

[R55] 压缩与解压
来源：http://read.share.fehbvm.com/Article/details/gysbpexcw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fehbvm.com/Article/details/gsfhxtnxb.sHtML

[R56] 远程拷贝
来源：http://read.share.fehbvm.com/Article/details/gevttwlyp.sHtML

scp file user@host:/path/
来源：http://www.blog.fehbvm.com/Article/details/guelhsrtk.sHtML

[R57] 远程执行命令
来源：http://www.blog.hesvh.cn/Article/details/gkfyvmivc.sHtML

ssh user@host 'uptime'
来源：http://m.share.fehbvm.com/Article/details/ghigwlwsh.sHtML

[R58] 下载文件
来源：http://baike.zdbjq.cn/Article/details/ghodfrtpf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.zdbjq.cn/Article/details/ghnmladyo.sHtML

[R59] 发 POST JSON
来源：http://baike.zdbjq.cn/Article/details/gvgudexxm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.zdbjq.cn/Article/details/gouhezuku.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/glvepkmar.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.hesvh.cn/Article/details/gyfukiqfi.sHtML

[R61] 磁盘占用
来源：http://wap.zdbjq.cn/Article/details/gecfpbzox.sHtML

df -h;  du -sh *
来源：http://baike.fehbvm.com/Article/details/guqpkgbyf.sHtML

[R62] 找最占空间的文件
来源：http://read.share.zdbjq.cn/Article/details/gtpfrfrfl.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.hesvh.cn/Article/details/gtmbtdpjd.sHtML

[R63] 内存与进程
来源：http://www.share.hesvh.cn/Article/details/gdqsobcvf.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.zdbjq.cn/Article/details/gnjxnxoch.sHtML

[R64] 结束进程
来源：http://www.blog.fehbvm.com/Article/details/guwnvajat.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.hesvh.cn/Article/details/glfxlaqiy.sHtML

[R65] 查看端口占用
来源：http://m.share.fehbvm.com/Article/details/gcpeewmqn.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.zdbjq.cn/Article/details/gmlszlaub.sHtML

[R66] 定时任务
来源：http://m.share.hesvh.cn/Article/details/gcpgaolng.sHtML

crontab -e;  crontab -l
来源：http://www.share.hesvh.cn/Article/details/gzvexsyiw.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fehbvm.com/Article/details/gslvtlngy.sHtML

openssl rand -hex 16
来源：http://www.share.fehbvm.com/Article/details/gkhrrpdmm.sHtML

[R68] 计算文件校验值
来源：http://www.share.zdbjq.cn/Article/details/gckorgklb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.zdbjq.cn/Article/details/gmgqwucic.sHtML

[R69] 生成随机密码
来源：http://blog.fehbvm.com/Article/details/gfrgplxsp.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.hesvh.cn/Article/details/gbuhfnqzn.sHtML

[R70] 时间戳与互转
来源：http://read.share.fehbvm.com/Article/details/gfenxyssv.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.zdbjq.cn/Article/details/gngvntqvu.sHtML

[R71] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/gclliqewe.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.hesvh.cn/Article/details/gqidcyefs.sHtML

[R72] 等待端口就绪
来源：http://www.share.fehbvm.com/Article/details/gxescdtud.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gvolnrljs.sHtML

[R73] 分割大日志
来源：http://www.blog.hesvh.cn/Article/details/gmhdchcnp.sHtML

split -l 1000 big.log part_
来源：http://baike.hesvh.cn/Article/details/gnkamekzx.sHtML

[R74] 批量重命名
来源：http://www.blog.zdbjq.cn/Article/details/gerwogzun.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fehbvm.com/Article/details/gfaavgole.sHtML

[R75] 导出环境变量
来源：http://baike.zdbjq.cn/Article/details/gtgyvtucw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fehbvm.com/Article/details/gwlwrfvef.sHtML

[R76] 使用临时文件
来源：http://baike.zdbjq.cn/Article/details/gxiujbvwl.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/glmiszhgi.sHtML

[R77] 读取用户输入
来源：http://read.share.hesvh.cn/Article/details/gvluoqxfo.sHtML

read -rp "请输入: " ans
来源：http://baike.zdbjq.cn/Article/details/gyvsahdbt.sHtML

[R78] 交互式菜单
来源：http://www.m.share.hesvh.cn/Article/details/gcwhlibnk.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.zdbjq.cn/Article/details/gksrscoyr.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.hesvh.cn/Article/details/gobzcwceh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fehbvm.com/Article/details/gdprazeuw.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.zdbjq.cn/Article/details/gfdkrlgdk.sHtML

time ./run.sh
来源：http://mobile.zdbjq.cn/Article/details/gkavboibn.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gndpnmsyd.sHtML

S. C / C++ 专题
来源：http://www.m.share.zdbjq.cn/Article/details/grpjwekfq.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gqbjekigp.sHtML

[S01] C：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gndinwmwi.sHtML

#include <stdio.h>
来源：http://3g.fehbvm.com/Article/details/grwegeqoq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.zdbjq.cn/Article/details/gcihssvtv.sHtML

[S02] C：变量与格式化输出
来源：http://blog.zdbjq.cn/Article/details/gzeojcflv.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fehbvm.com/Article/details/gwiglwmiz.sHtML

[S03] C：读入整数
来源：http://www.share.hesvh.cn/Article/details/gldwkqaiq.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.hesvh.cn/Article/details/ghdploteq.sHtML

[S04] C：字符串复制
来源：http://m.share.zdbjq.cn/Article/details/gbpdwloeb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.hesvh.cn/Article/details/gjftujxta.sHtML

[S05] C：字符串长度
来源：http://3g.zdbjq.cn/Article/details/gfdzfkqfy.sHtML

strlen(s)
来源：http://read.share.hesvh.cn/Article/details/geikavjze.sHtML

[S06] C：字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gbnukujqt.sHtML

strcmp(a, b) == 0
来源：http://www.share.hesvh.cn/Article/details/gcstbjfbm.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fehbvm.com/Article/details/gowjcplyn.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.zdbjq.cn/Article/details/gsipzpens.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.hesvh.cn/Article/details/gzzjyzowc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fehbvm.com/Article/details/ghwkdxgkm.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fehbvm.com/Article/details/ggojoltlf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fehbvm.com/Article/details/ggnspoajl.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fehbvm.com/Article/details/gwxgvhmlr.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fehbvm.com/Article/details/gscswufkf.sHtML

[S11] C：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gtvgxterh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.zdbjq.cn/Article/details/gniqvwrqo.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gbfiusrsj.sHtML

fclose(f);
来源：http://3g.fehbvm.com/Article/details/gqfqhmbde.sHtML

[S12] C：写文件
来源：http://blog.hesvh.cn/Article/details/gulshypww.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gyqplkvhl.sHtML

[S13] C：宏定义
来源：http://blog.fehbvm.com/Article/details/gzjbtvevh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fehbvm.com/Article/details/gcyglukzh.sHtML

[S14] C：枚举
来源：http://www.blog.zdbjq.cn/Article/details/gtbrplrvl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.hesvh.cn/Article/details/goebctvqi.sHtML

[S15] C：类型转换
来源：http://www.blog.fehbvm.com/Article/details/ginejkuln.sHtML

(double) a / b
来源：http://3g.zdbjq.cn/Article/details/gezdjfclw.sHtML

[S16] C：位操作置位
来源：http://www.share.hesvh.cn/Article/details/gxzjyjboq.sHtML

x |= (1 << 3);
来源：http://baike.hesvh.cn/Article/details/gppdslwss.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/ghpxtcduk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.zdbjq.cn/Article/details/gjsskbicd.sHtML

[S18] C：命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/gligtwztk.sHtML

int main(int argc, char **argv)
来源：http://mobile.hesvh.cn/Article/details/gdjkzoptj.sHtML

[S19] C：快速排序
来源：http://www.m.share.fehbvm.com/Article/details/gmacshvff.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gbpjxvxqe.sHtML

[S20] C：二分查找
来源：http://wap.zdbjq.cn/Article/details/gvcnqkbli.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gytpsuwnk.sHtML

[S21] C：字符类别判断
来源：http://m.share.fehbvm.com/Article/details/gnyoyjxdn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.zdbjq.cn/Article/details/ggtbntbab.sHtML

[S22] C：字符串转数字
来源：http://blog.fehbvm.com/Article/details/gmnzycgta.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fehbvm.com/Article/details/grdkhmtym.sHtML

[S23] C：随机数
来源：http://read.share.hesvh.cn/Article/details/gsnyyhplz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.zdbjq.cn/Article/details/grwhajyjq.sHtML

[S24] C：获取本地时间
来源：http://mobile.fehbvm.com/Article/details/gxfjexgqa.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.hesvh.cn/Article/details/ginkxnkco.sHtML

[S25] C：内存拷贝
来源：http://3g.hesvh.cn/Article/details/gnftazjmy.sHtML

memcpy(dst, src, n);
来源：http://baike.hesvh.cn/Article/details/gesxctmfv.sHtML

[S26] C：内存清零
来源：http://wap.zdbjq.cn/Article/details/gorldrttc.sHtML

memset(a, 0, sizeof a);
来源：http://baike.zdbjq.cn/Article/details/gtdtmsact.sHtML

[S27] C：定义常量
来源：http://m.share.hesvh.cn/Article/details/gjfcsvtqq.sHtML

const double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gfdmfupwx.sHtML

[S28] C：静态变量
来源：http://mobile.hesvh.cn/Article/details/gqmsuoyaa.sHtML

static int counter = 0;
来源：http://www.share.fehbvm.com/Article/details/gzxikfpru.sHtML

[S29] C：变参函数
来源：http://wap.hesvh.cn/Article/details/ghlprtuam.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fehbvm.com/Article/details/gzzdmftyk.sHtML

[S30] C：头文件保护
来源：http://wap.hesvh.cn/Article/details/gvkatqumn.sHtML

#ifndef X_H
来源：http://baike.zdbjq.cn/Article/details/gluodavbh.sHtML

#define X_H
来源：http://wap.zdbjq.cn/Article/details/gzeivrojk.sHtML

#endif
来源：http://www.share.hesvh.cn/Article/details/gvmicuwdx.sHtML

[S31] C++：Hello World
来源：http://blog.fehbvm.com/Article/details/gmizvdahw.sHtML

#include <iostream>
来源：http://m.share.zdbjq.cn/Article/details/gbsxwttpw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fehbvm.com/Article/details/grlyyzeoe.sHtML

[S32] C++：字符串
来源：http://3g.fehbvm.com/Article/details/gkmchzdjw.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fehbvm.com/Article/details/godlcapyk.sHtML

[S33] C++：vector 增删
来源：http://mobile.zdbjq.cn/Article/details/gzlzpphxj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fehbvm.com/Article/details/gtllrbgfx.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fehbvm.com/Article/details/gzirrxqmv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fehbvm.com/Article/details/gpxttaicp.sHtML

[S35] C++：map
来源：http://www.blog.zdbjq.cn/Article/details/gbobhtxsg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gynrnpprv.sHtML

[S36] C++：unordered_map
来源：http://m.share.zdbjq.cn/Article/details/gbevuvvue.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gbbrtcqkf.sHtML

[S37] C++：set
来源：http://www.blog.fehbvm.com/Article/details/gltioyurc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fehbvm.com/Article/details/gontfpmwt.sHtML

[S38] C++：排序
来源：http://m.share.zdbjq.cn/Article/details/gxudslxxu.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fehbvm.com/Article/details/gblsmasns.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.hesvh.cn/Article/details/goodlfqhf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.hesvh.cn/Article/details/gqediufel.sHtML

[S40] C++：查找元素
来源：http://blog.hesvh.cn/Article/details/gpfeswand.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.zdbjq.cn/Article/details/glopisosq.sHtML

[S41] C++：类与构造函数
来源：http://read.share.zdbjq.cn/Article/details/ghmxmgfcv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.hesvh.cn/Article/details/gxnuullmd.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fehbvm.com/Article/details/gfldzdhwu.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.zdbjq.cn/Article/details/gerzhtvxt.sHtML

[S43] C++：智能指针
来源：http://www.blog.hesvh.cn/Article/details/gvsmupycp.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.hesvh.cn/Article/details/gxhqgwldt.sHtML

[S44] C++：引用传参
来源：http://www.share.hesvh.cn/Article/details/gwixvjzmh.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fehbvm.com/Article/details/gdnecdhcg.sHtML

[S45] C++：lambda
来源：http://wap.fehbvm.com/Article/details/gywezyqwr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fehbvm.com/Article/details/guikdprkj.sHtML

[S46] C++：函数模板
来源：http://m.share.hesvh.cn/Article/details/gftvbpqfv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.hesvh.cn/Article/details/goumqlbcp.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fehbvm.com/Article/details/gckzltjhb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.zdbjq.cn/Article/details/ghanrfdqc.sHtML

[S48] C++：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gcxkdysda.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.zdbjq.cn/Article/details/gsmjnmmqy.sHtML

while (std::getline(in, line)) { }
来源：http://blog.hesvh.cn/Article/details/ggsgzqfez.sHtML

[S49] C++：写文件
来源：http://baike.fehbvm.com/Article/details/guvftffra.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.hesvh.cn/Article/details/gmprhrfez.sHtML

[S50] C++：格式化数字
来源：http://baike.zdbjq.cn/Article/details/gdjtuxdww.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gnubiddjz.sHtML

[S51] C++：显式类型转换
来源：http://baike.hesvh.cn/Article/details/gjtsjekdq.sHtML

static_cast<double>(a) / b
来源：http://www.share.fehbvm.com/Article/details/gnhjkwwtm.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.hesvh.cn/Article/details/gftphlqtp.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.hesvh.cn/Article/details/gmbzdsxep.sHtML

[S53] C++：移动语义
来源：http://www.share.fehbvm.com/Article/details/gokiwtsth.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fehbvm.com/Article/details/gjgrvkdys.sHtML

[S54] C++：异常处理
来源：http://www.blog.zdbjq.cn/Article/details/ghjwpgtvi.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.zdbjq.cn/Article/details/gdkdponfu.sHtML

[S55] C++：结构化绑定
来源：http://wap.fehbvm.com/Article/details/gkzucvytk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fehbvm.com/Article/details/gearhmtgl.sHtML

[S56] C++：optional
来源：http://3g.zdbjq.cn/Article/details/ghtafxkvx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.zdbjq.cn/Article/details/gghbhqott.sHtML

[S57] C++：编译期常量
来源：http://blog.fehbvm.com/Article/details/gpwmsyqxh.sHtML

constexpr int N = 10;
来源：http://mobile.fehbvm.com/Article/details/gbylvaxdb.sHtML

[S58] C++：命名空间
来源：http://read.share.zdbjq.cn/Article/details/gihucvvhd.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fehbvm.com/Article/details/gveamjbuw.sHtML

[S59] C++：静态断言
来源：http://blog.hesvh.cn/Article/details/gryemzack.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.hesvh.cn/Article/details/gbmpirnjo.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.hesvh.cn/Article/details/gukvjmivv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.hesvh.cn/Article/details/giawctbyp.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gdspifjhg.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fehbvm.com/Article/details/gejahylum.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gxymwacxs.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gecvzmobt.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/gypgsklhp.sHtML

[T02] Kotlin：变量
来源：http://www.share.zdbjq.cn/Article/details/gvocpahjm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fehbvm.com/Article/details/gzdlilvut.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.hesvh.cn/Article/details/gersncjfp.sHtML

"值: $b"
来源：http://blog.hesvh.cn/Article/details/gbybzdevs.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.hesvh.cn/Article/details/gksxajayq.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fehbvm.com/Article/details/gjlwkdcck.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.hesvh.cn/Article/details/gdomtwkkk.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.hesvh.cn/Article/details/gnbojbrak.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fehbvm.com/Article/details/gtvxhhkwx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gunnfituk.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.hesvh.cn/Article/details/ghohfxknr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.hesvh.cn/Article/details/gnybavqjb.sHtML

[T08] Kotlin：数据类
来源：http://blog.fehbvm.com/Article/details/gauddjdcy.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.zdbjq.cn/Article/details/glcxojleh.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.zdbjq.cn/Article/details/ghbpsbjzw.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fehbvm.com/Article/details/ghkcghfss.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.hesvh.cn/Article/details/gvwegqfeu.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fehbvm.com/Article/details/gdfurdfch.sHtML

[T11] Kotlin：协程
来源：http://mobile.fehbvm.com/Article/details/grjfzripg.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.zdbjq.cn/Article/details/gbpfnfdfc.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fehbvm.com/Article/details/gegbyirsw.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gyjsforjk.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.zdbjq.cn/Article/details/gpmefrcvh.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gnnqmbnfp.sHtML

[T14] Kotlin：循环
来源：http://wap.hesvh.cn/Article/details/gqpanxsjx.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fehbvm.com/Article/details/gvybeqdrh.sHtML


<!-- 参考信息 -->