代发 wailian999

esac
来源：http://3g.hesvh.cn/Article/details/gzncalegg.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fehbvm.com/Article/details/gcycbtkem.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fehbvm.com/Article/details/gaagemeal.sHtML

[R13] for 计数循环
来源：http://www.m.share.hesvh.cn/Article/details/gqbuymmbh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/gqoujtcxt.sHtML

[R14] C 风格 for
来源：http://www.m.share.hesvh.cn/Article/details/gwvpimvgr.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/gaseuuhhm.sHtML

[R15] while 逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gvbugqcml.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.hesvh.cn/Article/details/gtvbmvgva.sHtML

[R16] until 等待条件
来源：http://wap.fehbvm.com/Article/details/grmkwwxht.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/gptrhonnr.sHtML

[R17] 数组定义与取值
来源：http://3g.fehbvm.com/Article/details/gaanjcwmb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.hesvh.cn/Article/details/gjinuiumo.sHtML

[R18] 遍历数组
来源：http://3g.fehbvm.com/Article/details/gnnqnmkdi.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.hesvh.cn/Article/details/ggbbskofx.sHtML

[R19] 数组长度
来源：http://www.share.zdbjq.cn/Article/details/gpknrbweo.sHtML

echo "${#arr[@]}"
来源：http://3g.fehbvm.com/Article/details/gdbxzjakp.sHtML

[R20] 关联数组（字典）
来源：http://blog.fehbvm.com/Article/details/gmhelyumg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fehbvm.com/Article/details/goynxchke.sHtML

[R21] 字符串长度
来源：http://mobile.zdbjq.cn/Article/details/gogmurwuc.sHtML

echo "${#s}"
来源：http://www.blog.fehbvm.com/Article/details/gvukbuxla.sHtML

[R22] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/gttaydzhc.sHtML

echo "${s:0:5}"
来源：http://read.share.zdbjq.cn/Article/details/ggfwrogwg.sHtML

[R23] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gwqxmoegw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.hesvh.cn/Article/details/gntayztvw.sHtML

[R24] 大小写转换
来源：http://blog.hesvh.cn/Article/details/grauzgjjr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fehbvm.com/Article/details/gsxuulcnj.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.hesvh.cn/Article/details/gvdrvjdzz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fehbvm.com/Article/details/gzejavrfe.sHtML

[R26] 命令替换
来源：http://www.share.fehbvm.com/Article/details/gxlczdtzc.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.hesvh.cn/Article/details/gptacwfxj.sHtML

[R27] 算术展开
来源：http://www.m.share.fehbvm.com/Article/details/gajhycggh.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.zdbjq.cn/Article/details/gumsmhapz.sHtML

[R28] 浮点运算
来源：http://mobile.fehbvm.com/Article/details/gmgplflbt.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.hesvh.cn/Article/details/gxirvpsfd.sHtML

[R29] 定义函数
来源：http://3g.hesvh.cn/Article/details/gvoixdwdw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.zdbjq.cn/Article/details/gjwqrkdqm.sHtML

[R30] 函数返回状态码
来源：http://wap.hesvh.cn/Article/details/gzbpgxquq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.zdbjq.cn/Article/details/gxibkmfxv.sHtML

[R31] 局部变量
来源：http://www.m.share.fehbvm.com/Article/details/ghyiofyee.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fehbvm.com/Article/details/ghivloant.sHtML

[R32] 参数个数校验
来源：http://3g.hesvh.cn/Article/details/gcbbbenlo.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/gbulhuffz.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fehbvm.com/Article/details/gohwjtful.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.zdbjq.cn/Article/details/gpcokdtlx.sHtML

[R34] 退出时清理
来源：http://3g.zdbjq.cn/Article/details/gamnfqoah.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gyajkdzqe.sHtML

[R35] 后台执行并等待
来源：http://read.share.zdbjq.cn/Article/details/gjeraasco.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.hesvh.cn/Article/details/gbeeyyqdn.sHtML

[R36] 并发执行多个任务
来源：http://blog.fehbvm.com/Article/details/gaeuaunzt.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.zdbjq.cn/Article/details/gfhfgafeh.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fehbvm.com/Article/details/gnrxtzntw.sHtML

files=$(ls -1)
来源：http://www.m.share.zdbjq.cn/Article/details/gbbxddepj.sHtML

[R38] 管道串联
来源：http://www.blog.hesvh.cn/Article/details/gissyegvf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fehbvm.com/Article/details/grngnyejc.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.hesvh.cn/Article/details/guclxpvot.sHtML

cmd > out.log 2>&1
来源：http://blog.hesvh.cn/Article/details/gjzsbhbmt.sHtML

[R40] 追加写日志
来源：http://www.m.share.fehbvm.com/Article/details/gbxpbxqmr.sHtML

echo "log" >> out.log
来源：http://3g.hesvh.cn/Article/details/gqbhtbjdk.sHtML

[R41] 丢弃输出
来源：http://www.blog.fehbvm.com/Article/details/gwfmbioyy.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fehbvm.com/Article/details/gwpcimaec.sHtML

[R42] 输入重定向
来源：http://baike.zdbjq.cn/Article/details/gbbyeuich.sHtML

wc -l < a.txt
来源：http://wap.fehbvm.com/Article/details/gvnjkqdsm.sHtML

[R43] 按名字查找文件
来源：http://www.share.zdbjq.cn/Article/details/gogxilhte.sHtML

find . -name "*.log" -type f
来源：http://baike.zdbjq.cn/Article/details/gnlnjjobr.sHtML

[R44] 按修改时间查找
来源：http://mobile.hesvh.cn/Article/details/gxsvaiyok.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fehbvm.com/Article/details/gyswtwzdf.sHtML

[R45] 批量删除
来源：http://read.share.hesvh.cn/Article/details/gminbloqa.sHtML

find . -name "*.tmp" -delete
来源：http://baike.hesvh.cn/Article/details/gmikwcnxo.sHtML

[R46] 递归替换文件内容
来源：http://m.share.hesvh.cn/Article/details/gxmdxbjiy.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fehbvm.com/Article/details/gnveoauvc.sHtML

[R47] sed 单行替换
来源：http://3g.hesvh.cn/Article/details/gycahmuja.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gshzhmfub.sHtML

[R48] awk 取指定列
来源：http://blog.fehbvm.com/Article/details/gelkzhjmi.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fehbvm.com/Article/details/gaxjfvcfm.sHtML

[R49] awk 带条件
来源：http://mobile.hesvh.cn/Article/details/gjpmtdcsx.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fehbvm.com/Article/details/ggqwxhkcj.sHtML

[R50] awk 求和
来源：http://mobile.hesvh.cn/Article/details/guxoqbecg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.zdbjq.cn/Article/details/gklzkupix.sHtML

[R51] 排序去重取前几
来源：http://m.share.fehbvm.com/Article/details/gsyvmhqyt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.zdbjq.cn/Article/details/gijelhcid.sHtML

[R52] 统计行数
来源：http://www.blog.fehbvm.com/Article/details/gwcsrlhru.sHtML

wc -l a.txt
来源：http://mobile.hesvh.cn/Article/details/gjfbybqbr.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.zdbjq.cn/Article/details/gvkzifpxb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.hesvh.cn/Article/details/gjqaxjsws.sHtML

[R54] 比较两个文件
来源：http://wap.fehbvm.com/Article/details/guceqtblk.sHtML

diff a.txt b.txt
来源：http://baike.hesvh.cn/Article/details/gkrqylbsb.sHtML

[R55] 压缩与解压
来源：http://3g.zdbjq.cn/Article/details/gimevpoha.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.zdbjq.cn/Article/details/guqdounjv.sHtML

[R56] 远程拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gsjgxolib.sHtML

scp file user@host:/path/
来源：http://3g.fehbvm.com/Article/details/gszawxoge.sHtML

[R57] 远程执行命令
来源：http://3g.fehbvm.com/Article/details/goryaziol.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fehbvm.com/Article/details/gfsevqgbu.sHtML

[R58] 下载文件
来源：http://www.blog.zdbjq.cn/Article/details/gbuenszoc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fehbvm.com/Article/details/gfzvvcxtg.sHtML

[R59] 发 POST JSON
来源：http://wap.zdbjq.cn/Article/details/gxmojakfq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.hesvh.cn/Article/details/grqgnnbbl.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/gkjneerip.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fehbvm.com/Article/details/gquivksen.sHtML

[R61] 磁盘占用
来源：http://blog.zdbjq.cn/Article/details/gykjuugve.sHtML

df -h;  du -sh *
来源：http://www.share.hesvh.cn/Article/details/gnuzfwico.sHtML

[R62] 找最占空间的文件
来源：http://wap.fehbvm.com/Article/details/gmvgkklgn.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.zdbjq.cn/Article/details/gyucoygvk.sHtML

[R63] 内存与进程
来源：http://wap.hesvh.cn/Article/details/gzimzowlh.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.hesvh.cn/Article/details/gxpmcakpd.sHtML

[R64] 结束进程
来源：http://3g.fehbvm.com/Article/details/gfvsdsvux.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.zdbjq.cn/Article/details/gvyegtdri.sHtML

[R65] 查看端口占用
来源：http://baike.hesvh.cn/Article/details/gaowqxazr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fehbvm.com/Article/details/gyllqurun.sHtML

[R66] 定时任务
来源：http://www.m.share.fehbvm.com/Article/details/gbdskypzy.sHtML

crontab -e;  crontab -l
来源：http://baike.hesvh.cn/Article/details/gkxychlil.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.zdbjq.cn/Article/details/gwosyndcg.sHtML

openssl rand -hex 16
来源：http://3g.hesvh.cn/Article/details/gkvzhskxv.sHtML

[R68] 计算文件校验值
来源：http://baike.hesvh.cn/Article/details/ghyjijvim.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.zdbjq.cn/Article/details/gxgpwloia.sHtML

[R69] 生成随机密码
来源：http://blog.fehbvm.com/Article/details/grqosgwsj.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.hesvh.cn/Article/details/gsmchqjoz.sHtML

[R70] 时间戳与互转
来源：http://blog.hesvh.cn/Article/details/gczujhurz.sHtML

date +%s;  date -d @1700000000
来源：http://wap.zdbjq.cn/Article/details/gwpcgqczq.sHtML

[R71] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/gclplpjyd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fehbvm.com/Article/details/glfjcrfek.sHtML

[R72] 等待端口就绪
来源：http://www.share.zdbjq.cn/Article/details/gxazrwmqe.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/gojapomrw.sHtML

[R73] 分割大日志
来源：http://wap.hesvh.cn/Article/details/gkrsnpzmp.sHtML

split -l 1000 big.log part_
来源：http://wap.fehbvm.com/Article/details/gzkwgzzuv.sHtML

[R74] 批量重命名
来源：http://blog.fehbvm.com/Article/details/gpcyrzgqa.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.zdbjq.cn/Article/details/gsdtqrlmb.sHtML

[R75] 导出环境变量
来源：http://www.share.fehbvm.com/Article/details/gzziiptjh.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.hesvh.cn/Article/details/gxjptzycx.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fehbvm.com/Article/details/gnoaflgft.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gsymcdqko.sHtML

[R77] 读取用户输入
来源：http://blog.zdbjq.cn/Article/details/gkkizgoux.sHtML

read -rp "请输入: " ans
来源：http://m.share.fehbvm.com/Article/details/gucjwdmez.sHtML

[R78] 交互式菜单
来源：http://m.share.zdbjq.cn/Article/details/gpxfbezqs.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.hesvh.cn/Article/details/gpommblwd.sHtML

[R79] 解析命令行选项
来源：http://baike.hesvh.cn/Article/details/gvuubhbny.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.hesvh.cn/Article/details/gwujnkwbs.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.hesvh.cn/Article/details/gdlpedumi.sHtML

time ./run.sh
来源：http://blog.fehbvm.com/Article/details/gdldrzund.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ghxthsduh.sHtML

S. C / C++ 专题
来源：http://wap.zdbjq.cn/Article/details/gxvsevdei.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gdlkrmpqr.sHtML

[S01] C：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gtvuoofeo.sHtML

#include <stdio.h>
来源：http://www.share.fehbvm.com/Article/details/gnadlggjj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fehbvm.com/Article/details/gevamzgmf.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fehbvm.com/Article/details/gtebmwwvm.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.zdbjq.cn/Article/details/gsfyvhxri.sHtML

[S03] C：读入整数
来源：http://baike.hesvh.cn/Article/details/gnpnslzci.sHtML

int x; scanf("%d", &x);
来源：http://wap.fehbvm.com/Article/details/gafjujrrg.sHtML

[S04] C：字符串复制
来源：http://3g.hesvh.cn/Article/details/ghbzcvorf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fehbvm.com/Article/details/grappmkpt.sHtML

[S05] C：字符串长度
来源：http://mobile.zdbjq.cn/Article/details/gkinrlecd.sHtML

strlen(s)
来源：http://m.share.hesvh.cn/Article/details/gfohnjhlb.sHtML

[S06] C：字符串比较
来源：http://3g.hesvh.cn/Article/details/gknmwezcw.sHtML

strcmp(a, b) == 0
来源：http://3g.zdbjq.cn/Article/details/guiejejqd.sHtML

[S07] C：数组遍历求和
来源：http://blog.fehbvm.com/Article/details/gffnzpaor.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.hesvh.cn/Article/details/gycajrvwt.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.zdbjq.cn/Article/details/gdopadulg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.zdbjq.cn/Article/details/gxuyuhysr.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.hesvh.cn/Article/details/gejgkwhxz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.zdbjq.cn/Article/details/godamofew.sHtML

[S10] C：指针与解引用
来源：http://read.share.zdbjq.cn/Article/details/gwflxbesq.sHtML

int *p = &a;  *p = 5;
来源：http://blog.hesvh.cn/Article/details/gdwmvfrlb.sHtML

[S11] C：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gkbxhrnvj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.hesvh.cn/Article/details/gwqjimdwh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.hesvh.cn/Article/details/gtxxzwpph.sHtML

fclose(f);
来源：http://baike.fehbvm.com/Article/details/ggcgisala.sHtML

[S12] C：写文件
来源：http://read.share.hesvh.cn/Article/details/gaiairxyc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gjvoqdcmj.sHtML

[S13] C：宏定义
来源：http://blog.fehbvm.com/Article/details/gvsdmkcwe.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fehbvm.com/Article/details/gnistdlyb.sHtML

[S14] C：枚举
来源：http://www.m.share.hesvh.cn/Article/details/gismgebtl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.hesvh.cn/Article/details/gndvzuqxq.sHtML

[S15] C：类型转换
来源：http://blog.zdbjq.cn/Article/details/guipvznfn.sHtML

(double) a / b
来源：http://www.share.hesvh.cn/Article/details/grpjskbpd.sHtML

[S16] C：位操作置位
来源：http://baike.fehbvm.com/Article/details/glpfzlglx.sHtML

x |= (1 << 3);
来源：http://blog.zdbjq.cn/Article/details/gqwpqdyyn.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gicrgwrbu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.zdbjq.cn/Article/details/gwbeujsad.sHtML

[S18] C：命令行参数
来源：http://wap.zdbjq.cn/Article/details/gjkmjjglh.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.zdbjq.cn/Article/details/gaajchnjp.sHtML

[S19] C：快速排序
来源：http://baike.fehbvm.com/Article/details/gbqavazcq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gjunippfp.sHtML

[S20] C：二分查找
来源：http://mobile.fehbvm.com/Article/details/grjgxjffd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gftgozxap.sHtML

[S21] C：字符类别判断
来源：http://baike.fehbvm.com/Article/details/gywctxmqh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.zdbjq.cn/Article/details/gvnywzxzy.sHtML

[S22] C：字符串转数字
来源：http://wap.zdbjq.cn/Article/details/gcnprljjg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fehbvm.com/Article/details/goqptjmmx.sHtML

[S23] C：随机数
来源：http://www.blog.hesvh.cn/Article/details/gzggcahko.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fehbvm.com/Article/details/gvvnbgwbg.sHtML

[S24] C：获取本地时间
来源：http://blog.fehbvm.com/Article/details/gxxslfeyn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fehbvm.com/Article/details/grvlkbetk.sHtML

[S25] C：内存拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gbegfttjm.sHtML

memcpy(dst, src, n);
来源：http://baike.zdbjq.cn/Article/details/grnhkoals.sHtML

[S26] C：内存清零
来源：http://baike.zdbjq.cn/Article/details/gucikyrvx.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fehbvm.com/Article/details/gozlmtptx.sHtML

[S27] C：定义常量
来源：http://wap.zdbjq.cn/Article/details/gelhazabo.sHtML

const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gdmwefwrf.sHtML

[S28] C：静态变量
来源：http://3g.zdbjq.cn/Article/details/gqfogdrox.sHtML

static int counter = 0;
来源：http://mobile.hesvh.cn/Article/details/gubrkpdat.sHtML

[S29] C：变参函数
来源：http://wap.fehbvm.com/Article/details/gydbavqqa.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fehbvm.com/Article/details/gzlmfhzqx.sHtML

[S30] C：头文件保护
来源：http://www.m.share.zdbjq.cn/Article/details/gejnbxpfq.sHtML

#ifndef X_H
来源：http://www.share.zdbjq.cn/Article/details/gvidloton.sHtML

#define X_H
来源：http://www.blog.zdbjq.cn/Article/details/groclwxbz.sHtML

#endif
来源：http://baike.fehbvm.com/Article/details/gztohuqrb.sHtML

[S31] C++：Hello World
来源：http://3g.zdbjq.cn/Article/details/gmacyncuy.sHtML

#include <iostream>
来源：http://mobile.hesvh.cn/Article/details/gyqcqxafi.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.hesvh.cn/Article/details/gvggrozfy.sHtML

[S32] C++：字符串
来源：http://wap.zdbjq.cn/Article/details/gxldpjinc.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fehbvm.com/Article/details/grxtyawgm.sHtML

[S33] C++：vector 增删
来源：http://3g.fehbvm.com/Article/details/gzoqumlnh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gxpgybyob.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.zdbjq.cn/Article/details/gmfrdexii.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fehbvm.com/Article/details/gbnezxvkk.sHtML

[S35] C++：map
来源：http://wap.zdbjq.cn/Article/details/guxaeywai.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/gmgvnmagk.sHtML

[S36] C++：unordered_map
来源：http://3g.fehbvm.com/Article/details/gpmxkcelq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gttrpjkvt.sHtML

[S37] C++：set
来源：http://read.share.fehbvm.com/Article/details/gqwvbfiwb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fehbvm.com/Article/details/geqpuqknd.sHtML

[S38] C++：排序
来源：http://mobile.fehbvm.com/Article/details/gryjknnbs.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.zdbjq.cn/Article/details/gffeglqvf.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.zdbjq.cn/Article/details/gutrnwxur.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.hesvh.cn/Article/details/gkamrxrsf.sHtML

[S40] C++：查找元素
来源：http://m.share.fehbvm.com/Article/details/gbkwwhmbk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fehbvm.com/Article/details/goihvjnjo.sHtML

[S41] C++：类与构造函数
来源：http://read.share.zdbjq.cn/Article/details/gaxqecmml.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fehbvm.com/Article/details/gnmmvjyat.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.zdbjq.cn/Article/details/gzqgespan.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.hesvh.cn/Article/details/glcugjizp.sHtML

[S43] C++：智能指针
来源：http://www.share.fehbvm.com/Article/details/gtesrwvzn.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.zdbjq.cn/Article/details/ggoitbmyu.sHtML

[S44] C++：引用传参
来源：http://mobile.fehbvm.com/Article/details/ghljmnawb.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.zdbjq.cn/Article/details/gkydypwkm.sHtML

[S45] C++：lambda
来源：http://baike.fehbvm.com/Article/details/gpklkunym.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.hesvh.cn/Article/details/gzisgpxbx.sHtML

[S46] C++：函数模板
来源：http://www.share.fehbvm.com/Article/details/ghqrqyizw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fehbvm.com/Article/details/gqpdlcysw.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.zdbjq.cn/Article/details/galacekos.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.hesvh.cn/Article/details/gitxjwhfm.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gvwybthba.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fehbvm.com/Article/details/ghkqnvrmq.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fehbvm.com/Article/details/gbpjoxalu.sHtML

[S49] C++：写文件
来源：http://3g.zdbjq.cn/Article/details/gfbfuijge.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.hesvh.cn/Article/details/gvpcamswu.sHtML

[S50] C++：格式化数字
来源：http://wap.hesvh.cn/Article/details/gryrgfitt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gbxdsxuct.sHtML

[S51] C++：显式类型转换
来源：http://mobile.zdbjq.cn/Article/details/gpotcobgh.sHtML

static_cast<double>(a) / b
来源：http://baike.zdbjq.cn/Article/details/ggkodvyiv.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.hesvh.cn/Article/details/gtjgpslgz.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.hesvh.cn/Article/details/ghnzzhsgk.sHtML

[S53] C++：移动语义
来源：http://read.share.zdbjq.cn/Article/details/gotdranor.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.zdbjq.cn/Article/details/gxqasdchd.sHtML

[S54] C++：异常处理
来源：http://m.share.zdbjq.cn/Article/details/gvngbtwju.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.hesvh.cn/Article/details/glcuropec.sHtML

[S55] C++：结构化绑定
来源：http://mobile.hesvh.cn/Article/details/grlprbxes.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.hesvh.cn/Article/details/gtbxbouot.sHtML

[S56] C++：optional
来源：http://mobile.hesvh.cn/Article/details/gpbcjbqfc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fehbvm.com/Article/details/gfwfqlzwx.sHtML

[S57] C++：编译期常量
来源：http://www.share.fehbvm.com/Article/details/gjxavbzaw.sHtML

constexpr int N = 10;
来源：http://3g.fehbvm.com/Article/details/glbfoxzii.sHtML

[S58] C++：命名空间
来源：http://www.share.zdbjq.cn/Article/details/gpjlksnlm.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.hesvh.cn/Article/details/gxkydutgi.sHtML

[S59] C++：静态断言
来源：http://3g.fehbvm.com/Article/details/gxkpbqjkp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fehbvm.com/Article/details/glydkcvqi.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.hesvh.cn/Article/details/galunrtlr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fehbvm.com/Article/details/gtjkffqwn.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gwsewwlxj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.zdbjq.cn/Article/details/gwvodemdv.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gbdtfcgoi.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.zdbjq.cn/Article/details/grztgiepj.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gxnebvmyh.sHtML

[T02] Kotlin：变量
来源：http://baike.fehbvm.com/Article/details/gcyohfqed.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.hesvh.cn/Article/details/gzcgzumjf.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.hesvh.cn/Article/details/gasyofbiw.sHtML

"值: $b"
来源：http://3g.hesvh.cn/Article/details/gwcocubnf.sHtML

[T04] Kotlin：空安全
来源：http://3g.zdbjq.cn/Article/details/gqoscyqxb.sHtML

val n: String? = null;  n?.length
来源：http://wap.hesvh.cn/Article/details/gcgkoqgxf.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.zdbjq.cn/Article/details/gptbrupef.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fehbvm.com/Article/details/gqtzbxgvq.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fehbvm.com/Article/details/ggyltrpom.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.hesvh.cn/Article/details/gjjbvmoow.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.hesvh.cn/Article/details/gombuknug.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.zdbjq.cn/Article/details/gbhglgeta.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.zdbjq.cn/Article/details/gpxrfvwio.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fehbvm.com/Article/details/gcprnravx.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.hesvh.cn/Article/details/ggbvuxwmm.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.zdbjq.cn/Article/details/gbohsnlrn.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fehbvm.com/Article/details/gsgtjuzke.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.hesvh.cn/Article/details/gfyaevkox.sHtML

[T11] Kotlin：协程
来源：http://mobile.hesvh.cn/Article/details/ghrswknpi.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fehbvm.com/Article/details/gvuxuakfi.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.hesvh.cn/Article/details/gddnfvynn.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gydokbmwr.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.zdbjq.cn/Article/details/gfwzfwayy.sHtML

val m = mapOf("a" to 1)
来源：http://wap.zdbjq.cn/Article/details/ghznioxkg.sHtML

[T14] Kotlin：循环
来源：http://baike.hesvh.cn/Article/details/gcbhvjkpf.sHtML

for (i in 1..10) println(i)
来源：http://wap.fehbvm.com/Article/details/gfpflaoiq.sHtML


<!-- 参考信息 -->