代发 wailian999

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3iltvydbf.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3jussfnsz.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3xxsgjppk.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3iyzwmcyj.html

esac
来源：http://www.52xcode.cn/Article/details/gt3zyxumnfc.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3bmfryjpe.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3axyzhuwt.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3daqchfru.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3pokxzeoh.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3wphvqheq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3zogiweal.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ockeocak.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3zejwpzgw.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3iwzpgiay.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3xpzqbbgc.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3vhthzaab.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3sforisin.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3tawpsyhg.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3qpfykgpn.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3tdmvbhpy.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3eubvenni.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3ytkdeqpp.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3bkxrnelx.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3evgimmex.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3jymqqtpj.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3yvhjgbpc.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3irbuciuo.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3qdcbxmbq.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3nxhdrplw.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3oihbxsoz.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3leefslzg.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3pndnkavp.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3jozqrsmb.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3oxnqunve.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3xczclvxj.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3gyjfbujz.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3swgexzzw.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3fztcdmvx.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3qkdikvdd.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3wlwxcifi.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3eeccrtgx.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3ysxwtzpe.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3sldbjzjh.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3kfduoegv.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cgeufmxr.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3mkvyzuur.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3lqitpume.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3sflpcnml.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3dkoirckr.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3wvpqrmha.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3jppcnxmb.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3pzydqjog.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3ddmszwkk.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3mvjxojpu.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3ukfsbzst.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3bavmkejl.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3jxehefbg.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3bqbqsiaq.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3anodttaj.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3qxrslmip.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3qnjbdric.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3lwualpew.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3qkjuppfd.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3usphlhdn.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3nwubkhao.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3vltglalo.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3lrutxhun.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3agxdvzop.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3vopqhzjj.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3lhfjhhuv.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3bouuuask.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3mbvjjlro.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3dutisgjp.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3hvfxtoub.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3jyybtojv.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3keeyqnyt.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3chjxzotf.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3haxfwmhj.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nqeitopa.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3drpotbev.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3mrzhqodd.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3viyeajux.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3exhbjyqg.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3gmnfsbip.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3rdwojgbk.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3fxiaxqip.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nlwdibgt.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3jwubsndk.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3vrcvdecu.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3znvawzyd.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3vipdughw.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3yvhidobd.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3ninfuajx.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3emalvfxi.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3kyabkejk.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3ylzptfgg.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3dcftghch.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3atndzykx.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3zpvxvnrg.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3yosdqkrh.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3svsheqjh.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3mgiosvdk.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3xweulquk.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3fpdzwssy.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3tezfexjq.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3ulfgrscz.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3riuqqvde.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3mdpaxrmw.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3gkvdtemk.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3admlcznt.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3mpadnogs.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3wsjxkthz.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3lzkjspms.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3hskdmqzs.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3zeuzpwof.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3audnyozn.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3iadoxwlc.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3vmlqtvga.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3utozucdh.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3zopdgdst.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3ehvrvoym.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3kvqmepna.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3wsraeeqz.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3abojxatr.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3bgjmbwhu.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3frcilcbe.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3umshmyqc.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3ewicwsfc.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3cuyhjcmr.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3gjndutff.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3kntmyren.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3zbkohokf.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3xioktpja.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3hlnfarje.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3zwqrxsok.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3fxykhslv.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3werlarfz.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3ezvscvnb.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3xgzeavfh.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3johaqkgv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3eycdmdjs.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3mgbyofak.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3ftbqyvdj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sbazcwck.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3koygmavh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mxezhyvb.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ajqgeadg.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3blhbfloj.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3jfvjbbpp.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3hqsoqjju.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3mwniakah.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3ppznbezs.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3ixbxwknf.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3yjhryawr.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3oqtwhmeo.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3aoxrlxvo.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vgrzpnyk.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3velaybsy.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3cmjvxhey.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3xoodjpsr.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3ddgvsqjj.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3kefnlcqn.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3hgzrxjzh.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3mmggvjzx.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3xpbvvatz.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3ntfiwdlo.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3iecacgnq.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3cjfqsnse.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3xetnnjqz.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3cntsbzhl.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3uhrsyyew.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3aazkncjo.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3tlvrjwjj.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3rnnlaqlh.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3utdancbn.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3qhptvxmi.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3rfuzggud.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3oduhkqht.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3diuejetx.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3pglvuoiu.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ejxtpkyf.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3yowchsjp.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3gafrtzoe.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3jlmfekzt.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3gpqourql.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3pherxhtr.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ravswsxr.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3cfpatcqb.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3qrmntunl.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3fjkjzmpr.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3rchabnsm.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3lnfsxile.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3fhqbesvc.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3tjkpctyn.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3gvchblyj.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3lngdhbnf.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3tgidpyqb.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3dcclsrjb.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3bqxzdlxn.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3kzfzoxae.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3siscdjoz.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3wndkpkpt.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ahfkzaoj.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3uoqmymxr.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3tzxksuov.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3yrvytahs.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3tubqiqxj.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3kctikdii.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3ihlphwdp.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3egbbuymg.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3pfcqtrwx.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3leojkfne.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3demsphir.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qhdxeory.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3xlhnnfyn.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3tibptbqz.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3tuowejbr.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3slvfpdki.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3wfvthgdp.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3ifrdhbic.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3tndmbttd.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3joawvlrc.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3oqlvbzgq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3bwmmxpcd.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3rehmkpvd.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3nmdtdvfo.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3mhxvnfao.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3apcbbpbx.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3qngpvxvk.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3jexzhrbh.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3lmxkausz.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kaclnklf.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3afunxuxw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3vfenbwzt.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3rdsarksh.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3wkkkapqv.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3meqitpgc.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3mbdukapw.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3zcutdmwn.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3xoirfjkx.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3qsutscll.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3zlsturjb.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3grljpquv.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jbybriwd.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kgspvxxg.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3xzpttrad.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3whuaindj.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3eonobojo.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3bcblwitz.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3jvbatmzj.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3lrwwskvz.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3hosckhqk.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3bzfrgubb.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3vlwqptcc.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3eycgjwie.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3mgcudbcu.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3ctkntdau.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3oiwqksze.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3xppsnbcw.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3uximypbv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3lnowzymw.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3qvrbcmki.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3urfdhrnv.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3jazezkoq.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3avssmwun.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3qepiacut.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3rkomrflh.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3hhmvpjsd.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3sejnnmvs.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3dhextoel.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3nrwydbnx.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3lirkilmc.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3isaeydhj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nrkbenmh.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3zzdtnuws.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lmxqjyuq.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hxzsjrvd.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ysozsasd.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3zmsnkszv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3idoeuket.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3qqtlfhot.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3auyzuikb.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3cfvrnasu.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3phdblncf.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3pogerquq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3hdnguahv.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3hmoviiju.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3dxhdswaz.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3oebkcbye.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3lksbdwlm.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3obyianjl.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3fijhnssg.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3nbwhnutl.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3mzhmknnt.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3icrccbpg.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3icunexsc.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3nexmbrlp.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3dainvopn.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3uneqasyz.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3sirjeacq.html


<!-- 参考信息 -->