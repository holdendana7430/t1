代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3ezfdpsej.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3lqmrdvbl.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3befacshp.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3iuocokxv.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3zqcxiebh.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3qnxejbwk.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3apllacjm.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3cwpjukkr.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3nbemkfcx.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3glcbzoxa.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ybxmdjyx.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ymibcskm.html

esac
来源：http://www.52xcode.cn/Article/details/gt3daqkgqlg.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3kwzoieyl.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3isathhmm.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3phftrytv.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3eiesshhi.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3ndngjqxj.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3gwuqawpe.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3oamrvtfa.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hnfjcomx.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3exiadukt.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3wltjpnic.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3hemrupkl.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3hgedixim.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3bhleqywu.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3pygcnyae.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3xvqxovst.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3znqwkgeb.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3psitrynx.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3fudbfkkh.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3sqkltsof.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3pjwkarxc.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3msejrzee.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3gjtlswxi.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3tdxpzhjy.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3vjxqpflk.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3lvzicueh.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3odmwvwcl.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3uxoaghge.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3bibqaprk.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3jbfffskc.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3bytiuxuu.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3bjlksjkd.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3grpafcyf.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3vaerhfig.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3kikvbwup.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3ubvpelxi.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3zyehvqdc.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3aiywetvg.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3tgiieiym.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3wxfxsyhc.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3foqukuls.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3ribdkfan.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ipdkubul.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3jddgyjzm.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3qxdlypyi.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3gpvrpuwi.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3jhizvuaa.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3xsnkhrbj.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3mpntousk.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3fyqzykby.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3zbmljkyn.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3lszmgzku.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3drtpunpd.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3rseqtpds.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3okxwqzcy.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3dvmxihmm.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3ccasslxf.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3athgprcb.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3krddckvx.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3cplilmia.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3hgebbwcx.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3kmxlvcbd.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cdxukosa.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3wuigojhc.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3wdnnvpum.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3ezeovczh.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3pkbtlkea.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3kzifxfye.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3bnpxawvl.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3wilizvxt.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3wpoauxuc.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3xsydxzfc.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3glvumkle.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3xlkvwhxl.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3fsfazlas.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3ylaojqul.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3zooppsdu.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3wlexllbd.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3sqiwlouc.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3igmdisgz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3fcdrkzhy.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3nxhijlea.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3sqsjucec.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3tztekusu.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3jrjgdeav.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3nptqtwqt.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3hcwhaurg.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3qkgiqejg.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3ohatqckl.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3frwxgvnb.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3yxukprix.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3zssuarph.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3kepiofip.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3fhilmgpz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3xjijcyzn.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3mcmpuvwt.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3sqwfomfg.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3vrbepnzr.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3rzbmcxjm.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3plimrpvi.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3xbsjchof.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3lqklonar.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3dbqykhpz.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3imvnzeic.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3snsijlvu.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3rtvkaahb.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3jrbneufu.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3vbtazwqb.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3sdhhvmea.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3fqusnior.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3gabelgvs.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3ycgplrax.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3svgssozs.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3vffiducv.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3oifyepob.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3dxbmrpwa.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3zdlbaelj.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3zixvdwkn.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3odmgodsj.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3aoypbple.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3fbgxehco.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3wutvaghs.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3vkwbqbrx.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3ciawmwnd.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3zfjpxxyu.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3psedvgzw.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3hqwxloph.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3covsvsnw.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3vfgxkwcz.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3uevanjnm.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3oahnmmyx.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3eclupvsp.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3diyhfznn.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3qqfrqxnl.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3qvticeke.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3lhulfpex.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3huzycdwa.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3afewfqqj.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3wbuqlnlb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bvorbdaz.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3jsegzuud.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kajozbza.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3casoktea.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3fyzrpmxq.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3gvpytpbs.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3rmgqtaye.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3hylnjmnz.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3lqegskiw.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3geffuahw.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3gjvyxslf.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3zoxfapnk.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3wkixsxkr.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lwczcrzb.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3kvsdrjcx.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3wqiqjlir.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3pabzdojr.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3epnvcpii.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3qzhuggas.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3gqorznfr.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3xcofggwi.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3oepccuuk.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3cdnvposg.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3eliivytx.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3sosleexh.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3dsburqlt.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3nweofyex.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3gtdbtnry.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3cahqytue.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3vorzyyzw.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3hbkccxcd.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3brdbxeqt.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3kkhebtcu.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3ngppiaqb.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3odmezyuy.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3zawhkoqp.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3jprfvyss.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3acwevsxs.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3auyqhwxy.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3zlhwfrra.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3djbkltul.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3cwtokolt.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3aankhela.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3vmcgwyqx.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3bsykhhtd.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3yydrhvmp.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3jaugjmfr.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3mskajatc.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3upyootdo.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3oukheuzi.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3rojgnnsp.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3uurfxhqu.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3klbnvrcc.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3wzzjqcrw.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3xcbaprzv.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3btthprah.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3rtrisgre.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3fqkcsraa.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3edvrzytr.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3clyzpobm.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3jnrzxnud.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3plelisgr.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3tnwuzefs.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3solvdabj.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3xnwgorfx.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3lgesqulu.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3vbggwyjq.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3vsblbadp.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3szlynhul.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3htdwuudm.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3rfcvfsna.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3answofhq.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3wzxnddye.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3knskxdge.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3nayqumlq.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3membjcch.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ozbuqinx.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3pzpfvcao.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3plfhcltw.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3dluyfiqp.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ukoqsveh.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3xoeowswj.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3wwxuzawq.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3nccghrnf.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3nnppzxbh.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3qoyfreiu.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3fzrrghko.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3tymjmhxq.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dmkmtbhl.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3wucvzrup.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3ifhmljcv.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3mlntueky.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3bywctkln.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3jcktbpxu.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3ghxvalqy.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3hskhpban.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3pvnvqrvk.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3elrrqidr.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3kjgfwqtl.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3bhlewimg.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3pjbokqiv.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ohxxjdza.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3kralzpvj.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3gucedwtv.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3mihvxprd.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3logrvgle.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3pjikesgm.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3hmriinrg.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3xyfwgeda.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3dydspkyo.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3ricnmgbc.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3kjgvvttb.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3mcjzvfkg.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3ndmpkkwn.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3fpoiweyl.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3sxakmilq.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3deekkfyj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3hpmnnuhr.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3fzgnzzcl.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3vszexdqw.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3tqckfhtw.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3fajadnij.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3bmomdklc.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3dfvjyxbs.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3dzokolqa.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3vunuufzx.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3wpdpjvsc.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3djwnwzqo.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3wjnjyegb.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3hdkgztkl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rbutbbhd.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3zsjhried.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3powikjfi.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zcooqdlv.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ooeavvwe.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3rbrcbewi.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3tairbuyq.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3owlmxikj.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3xggukxnx.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3gwuqxkns.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3ujmhfswg.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3aghjrhlo.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3eqrqjhzj.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3cpjoisvu.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3hllimotv.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3dotzmyir.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3uaggeaxc.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3dwjhipbk.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3aqzxjueb.html


<!-- 参考信息 -->