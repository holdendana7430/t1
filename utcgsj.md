代发 wailian999

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3rtuvxmsl.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3zfeylmgo.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ajwdpmpr.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3ywllnyrk.html

esac
来源：http://www.52xcode.cn/Article/details/gt3fftndynq.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3arflhnsw.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3zvlsnxwk.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3uxrgdouy.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3sbumkteg.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3kwltjuee.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3aiwkuzlg.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3uctfbudt.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lzocfsdg.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3fckifldf.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3idlzuxds.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3tkihccuf.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3cuaugrhh.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3clmwyzgu.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3vyevhgoq.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3xcsztdbf.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3tgdyrrsi.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3zhcjoqow.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3mbrvjvbz.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3oluhmkhr.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3jgglktfm.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3vbvrxyqg.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3yqmznmle.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3xwzurgyq.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3bkhwgehq.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3psyuosot.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3tzgvpfhx.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3ffzfltou.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3pwhjiobx.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3pbzryddu.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3leiqmkdx.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3mgrzklpp.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3qokasxki.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3echudjko.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3ptrlgfok.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3jtfyfklw.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3yhfrfknp.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3uzfudcbj.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3fcxmxzmp.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3yxwdwexb.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gpuxtlwq.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3pzemkldp.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3owohraid.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3qhrudlgj.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3wsmgusdi.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3rwexvxvh.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3vwvtcjdq.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3zpksssgb.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3dbfyvzlx.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3wjgijpae.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3qflpdvbv.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3wzrxuugx.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3fyxefakd.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3eiiwvukd.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3fcyrctnd.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3dcuvgfia.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3lmjlxfgr.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3hyjgnrzf.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3hbiaabha.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3kuttnzsy.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3nzbmoqnr.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3nvdnsmqq.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3alaqckox.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3gwiugctx.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3brferajn.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3vgnmvcrf.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3esmnuwvi.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3kuudaatj.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3vaoiixeh.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3ilufznet.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3tfyowthb.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3llystcqj.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ejecjdlq.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3gkvopgjl.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ajjsmwqq.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3ziamoddp.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3hwjhehrs.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3cpkhnzld.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3kajwduja.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3cullnjwz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3ombxjdpd.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3bwrfwtid.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cfqcepkh.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3gamkxyfz.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3slorvsfr.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3cfxgbmph.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jbzkzkbu.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3fioludic.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3kaczozzr.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3nsnrdnsa.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3qzskrlrk.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3clvuslew.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3drwkprmb.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3kbvmhrom.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3ofiuydyb.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3dkrlkeqc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3soshbzik.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3olwlbvxz.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3rxbmgyzp.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3ujjikjbe.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3vzuretwl.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3vheumlaf.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3aescueds.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3apnpifgx.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3tevidshy.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3wdjulsoh.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3mvkaijkb.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3lozawqvq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3eeemxkwn.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3fxreaysu.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3hbscytju.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3svgwtvnp.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3aldymsbo.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3newsmtxd.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3gmqxzont.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3asqdkqjx.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3pywangno.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3gcjgfxfw.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3spenxvfm.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3xuzqvlbv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3sutqhfbo.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3xixmrztl.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3ibyffzxi.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3uwxsccak.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3mavoplch.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3axfeohbq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3dwabiccf.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3tchtjebw.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3rexbkslx.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3cdzjoykk.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3btqcukin.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3tzqowcfq.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3ngiybphe.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3negnnazh.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3zwsqdygu.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3thxbixlj.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3gxluaggw.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3bunzpjyh.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3eyqlkhjf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qruqqmqb.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3alvsmbok.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ahzjkrsq.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xnnonnzd.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3pzwqjrjw.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3meyglwga.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3mmjoylrp.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3pivezhqb.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3rswhgxkt.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3suhbqepq.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3nltogoxl.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3znbrmmtt.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3paapccpv.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fmfrpnbt.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3dofinofe.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3awfhwkrq.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3uekwjuqk.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3pljyxrvu.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3hkenjywy.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3gmivbmfm.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3trwymtxi.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3femldhfw.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3kcstjehn.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3kyvdtxtb.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ylizwuya.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3uqbqqdpx.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3zwnpocdm.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3dytqiccs.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3icbxvruv.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3gomfvacw.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3qqmxdiof.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3tlqfnzbf.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3nkogqezx.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3xwajbeqv.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3lgflgfub.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3ukssojon.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3venxmsku.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wntisiag.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3xovberzj.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3asomldyl.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3fuztqawa.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3agxaeuun.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3jxwniiac.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3lpsjsyzj.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3njhyynlh.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3fquzdoif.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3wfpjtkhw.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3kjwhssbk.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3mgfazuop.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3wbptdyxw.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3axxaarrw.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3hjirduhi.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3krvrhgfa.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3asdsgvst.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3ziiwpuco.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3mccikacw.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3nawoerdj.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3wdshhjix.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3bntypqfr.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3pbnnfrzd.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3yyxwptjx.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3rvbomysc.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3tnuzdsdf.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3xbilrrbg.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3exdyobyf.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3quggkkdr.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3mzdjfwra.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3izmanpir.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ozbhzhbj.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3nikgusxt.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3dhxbdeiy.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3hjtezmpc.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3jsidawqf.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3wzhjseee.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3tgcxjrcu.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3yjljlxpk.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3xkmukjog.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3nffmtgzo.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3tiphrtpv.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3lcbwgyjt.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3xdrxlbje.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3ouupsqkg.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3wozzauyp.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3updtjsej.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3bnjeglrr.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3kcbcflla.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3tckrwjqm.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3fawlrrtm.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qveppzvu.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3grqrkoac.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3etluacxk.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3gajvmlcs.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3laaklwrf.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3rcfpucts.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3oehktywd.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3vyxizaqe.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3hrmcqvfc.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3gefecyhi.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3yupsxhpp.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3xpkpsnxm.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3tsoftmwr.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qonwsocq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3sejasvhh.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3sjscppqd.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3syllpbih.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3gvrnojem.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3wyjhjdem.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3rsdzxfpa.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3ttcwmawh.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3jplwwrss.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3dnhgacpv.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3dylxukxk.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3pjiafzcy.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3kvqreiec.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3mswuvfwl.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3ionleiog.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3pfgujine.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3fghftgvo.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3fbnmclze.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3aefvcbqe.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3weutfkxe.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3lvslnbud.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3mnasggod.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3bmusypgc.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3jgtsuftm.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3khpzjzte.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3mdvaayqp.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3utkkzola.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3acnzutor.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3uqwuyvtm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3plnyslmu.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3btixroqq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tfxcmfvj.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3fvpcgqek.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3eqgggvds.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3vybeswxm.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3povbewsx.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3wvugztns.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3mjmdcdbn.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3iwejghfu.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3dvcepgwn.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3ctsjqxzq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3dxcqfzjj.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3qfhkdwju.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3xkbnuhjf.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3vbzzfjgt.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3pzdlpipi.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3zwlepzlv.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3gdkuslap.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3cmwjific.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3eryqacni.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3rgsjfesq.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3uygyorls.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3jfxahttl.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3mxzgpirz.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3kuleozzl.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3rwlrpsik.html


<!-- 参考信息 -->