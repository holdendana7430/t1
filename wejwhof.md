代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.zdbjq.cn/Article/details/guvrybhua.sHtML

[R10] 正则匹配
来源：http://www.share.fehbvm.com/Article/details/gitsagqiu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.zdbjq.cn/Article/details/gnlvvbtle.sHtML

[R11] case 多分支
来源：http://m.share.hesvh.cn/Article/details/gedczwsqf.sHtML

case "$1" in
来源：http://www.share.hesvh.cn/Article/details/gxamlkfok.sHtML

start) echo "启动" ;;
来源：http://baike.hesvh.cn/Article/details/goxjsglyv.sHtML

stop)  echo "停止" ;;
来源：http://wap.zdbjq.cn/Article/details/gahhbfmpq.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gqxgntrez.sHtML

esac
来源：http://www.m.share.zdbjq.cn/Article/details/gmvjydpbq.sHtML

[R12] for 遍历文件
来源：http://mobile.fehbvm.com/Article/details/getmtalew.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.hesvh.cn/Article/details/gqolhsxwz.sHtML

[R13] for 计数循环
来源：http://www.share.fehbvm.com/Article/details/gnkkpvzrz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/gpbmbkene.sHtML

[R14] C 风格 for
来源：http://3g.hesvh.cn/Article/details/gpdqllhuk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/ggoreixnm.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/ghwbyrdun.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fehbvm.com/Article/details/gjoyfumse.sHtML

[R16] until 等待条件
来源：http://wap.hesvh.cn/Article/details/gbpwgdmyi.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gantvcnoz.sHtML

[R17] 数组定义与取值
来源：http://www.share.hesvh.cn/Article/details/gqsuzuwwu.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.zdbjq.cn/Article/details/gjysdfwit.sHtML

[R18] 遍历数组
来源：http://read.share.fehbvm.com/Article/details/gjpuyauvn.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.zdbjq.cn/Article/details/gisnndnxf.sHtML

[R19] 数组长度
来源：http://www.m.share.fehbvm.com/Article/details/gjewqdwxm.sHtML

echo "${#arr[@]}"
来源：http://read.share.zdbjq.cn/Article/details/ggkhcefaz.sHtML

[R20] 关联数组（字典）
来源：http://wap.hesvh.cn/Article/details/goguwkavv.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fehbvm.com/Article/details/ghmnmwtnk.sHtML

[R21] 字符串长度
来源：http://mobile.fehbvm.com/Article/details/gnjspmsgi.sHtML

echo "${#s}"
来源：http://wap.hesvh.cn/Article/details/gocmtgcwu.sHtML

[R22] 截取子串
来源：http://mobile.hesvh.cn/Article/details/gqrlqvupx.sHtML

echo "${s:0:5}"
来源：http://mobile.fehbvm.com/Article/details/ggpihxoll.sHtML

[R23] 字符串替换
来源：http://baike.zdbjq.cn/Article/details/ghojxlung.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fehbvm.com/Article/details/gmgtdrfpe.sHtML

[R24] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gkiofywpz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fehbvm.com/Article/details/gscfnomnt.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.hesvh.cn/Article/details/ghjhfjbpp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.hesvh.cn/Article/details/gijylhvul.sHtML

[R26] 命令替换
来源：http://mobile.hesvh.cn/Article/details/gzkurrrjr.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fehbvm.com/Article/details/gxbdipejq.sHtML

[R27] 算术展开
来源：http://read.share.hesvh.cn/Article/details/gzulqdhbm.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fehbvm.com/Article/details/gopdjziba.sHtML

[R28] 浮点运算
来源：http://www.blog.zdbjq.cn/Article/details/gnjxoouqo.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fehbvm.com/Article/details/grkfwrcan.sHtML

[R29] 定义函数
来源：http://www.share.zdbjq.cn/Article/details/guxdosorx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fehbvm.com/Article/details/gwmvuzuqq.sHtML

[R30] 函数返回状态码
来源：http://3g.zdbjq.cn/Article/details/grpfqmzgr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fehbvm.com/Article/details/gqoyqmdsk.sHtML

[R31] 局部变量
来源：http://3g.fehbvm.com/Article/details/gpeowkjva.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.zdbjq.cn/Article/details/gkkhvslcn.sHtML

[R32] 参数个数校验
来源：http://baike.zdbjq.cn/Article/details/ghvfkmjji.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/gwesznfqi.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.hesvh.cn/Article/details/ghzormwvw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.zdbjq.cn/Article/details/gjjqiwnrg.sHtML

[R34] 退出时清理
来源：http://blog.zdbjq.cn/Article/details/gzfiqfbau.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gzpcxkxgi.sHtML

[R35] 后台执行并等待
来源：http://baike.zdbjq.cn/Article/details/gdbsrpzgr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fehbvm.com/Article/details/gzqnieljr.sHtML

[R36] 并发执行多个任务
来源：http://mobile.hesvh.cn/Article/details/gslfhbnmu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.hesvh.cn/Article/details/gvzadkgcl.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fehbvm.com/Article/details/gvspsjyse.sHtML

files=$(ls -1)
来源：http://blog.fehbvm.com/Article/details/geihcosuz.sHtML

[R38] 管道串联
来源：http://mobile.hesvh.cn/Article/details/gmuzbdaok.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fehbvm.com/Article/details/gorhnrrcr.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fehbvm.com/Article/details/gdvdjhzkf.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gtgakrazv.sHtML

[R40] 追加写日志
来源：http://mobile.fehbvm.com/Article/details/grdilvved.sHtML

echo "log" >> out.log
来源：http://3g.hesvh.cn/Article/details/gfddgrned.sHtML

[R41] 丢弃输出
来源：http://wap.zdbjq.cn/Article/details/gfuovbgnk.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.hesvh.cn/Article/details/gmtjgpylr.sHtML

[R42] 输入重定向
来源：http://wap.fehbvm.com/Article/details/gaqtspjne.sHtML

wc -l < a.txt
来源：http://read.share.hesvh.cn/Article/details/guowewppj.sHtML

[R43] 按名字查找文件
来源：http://m.share.fehbvm.com/Article/details/gakkyefbo.sHtML

find . -name "*.log" -type f
来源：http://read.share.zdbjq.cn/Article/details/gvfyopuxf.sHtML

[R44] 按修改时间查找
来源：http://baike.fehbvm.com/Article/details/glsbegkdp.sHtML

find . -mtime -7 -type f
来源：http://www.share.zdbjq.cn/Article/details/gyvkhoult.sHtML

[R45] 批量删除
来源：http://wap.hesvh.cn/Article/details/ggksqyvqy.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fehbvm.com/Article/details/gefnufrhk.sHtML

[R46] 递归替换文件内容
来源：http://read.share.zdbjq.cn/Article/details/gqybjhjol.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fehbvm.com/Article/details/gqbwgqfef.sHtML

[R47] sed 单行替换
来源：http://m.share.hesvh.cn/Article/details/ggedstxsb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fehbvm.com/Article/details/gzusgrgiz.sHtML

[R48] awk 取指定列
来源：http://mobile.zdbjq.cn/Article/details/gvmowqncf.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gtasoyuih.sHtML

[R49] awk 带条件
来源：http://m.share.fehbvm.com/Article/details/ggrgsijqw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.zdbjq.cn/Article/details/gyjhzjwma.sHtML

[R50] awk 求和
来源：http://3g.fehbvm.com/Article/details/gdvuwvcxz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gouohimve.sHtML

[R51] 排序去重取前几
来源：http://www.blog.zdbjq.cn/Article/details/ggzboglsu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fehbvm.com/Article/details/gvrftdbzt.sHtML

[R52] 统计行数
来源：http://wap.zdbjq.cn/Article/details/gcanqhtyp.sHtML

wc -l a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gjtwdrdzu.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.hesvh.cn/Article/details/ggbqmytqu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.zdbjq.cn/Article/details/gpjfgbppj.sHtML

[R54] 比较两个文件
来源：http://blog.fehbvm.com/Article/details/gtlsaruwb.sHtML

diff a.txt b.txt
来源：http://www.m.share.hesvh.cn/Article/details/gxivyhxry.sHtML

[R55] 压缩与解压
来源：http://baike.hesvh.cn/Article/details/gfvvrrjbd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.hesvh.cn/Article/details/gfqctbzdq.sHtML

[R56] 远程拷贝
来源：http://blog.hesvh.cn/Article/details/gcjnpjnok.sHtML

scp file user@host:/path/
来源：http://m.share.zdbjq.cn/Article/details/gxwiqxigd.sHtML

[R57] 远程执行命令
来源：http://m.share.zdbjq.cn/Article/details/ggbfvffkt.sHtML

ssh user@host 'uptime'
来源：http://m.share.zdbjq.cn/Article/details/gljieczxg.sHtML

[R58] 下载文件
来源：http://www.m.share.hesvh.cn/Article/details/gdmuwdwhc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fehbvm.com/Article/details/ghzluqtlp.sHtML

[R59] 发 POST JSON
来源：http://blog.fehbvm.com/Article/details/gdxjkfziw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.zdbjq.cn/Article/details/gzpzxzfsu.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/gxebsjwbu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.zdbjq.cn/Article/details/grmxuuxcf.sHtML

[R61] 磁盘占用
来源：http://read.share.fehbvm.com/Article/details/gnctbnaum.sHtML

df -h;  du -sh *
来源：http://3g.hesvh.cn/Article/details/grkpehiac.sHtML

[R62] 找最占空间的文件
来源：http://wap.zdbjq.cn/Article/details/gxlkougwt.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.zdbjq.cn/Article/details/ggyxqfbne.sHtML

[R63] 内存与进程
来源：http://blog.zdbjq.cn/Article/details/gpahajput.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fehbvm.com/Article/details/gjxjjtafc.sHtML

[R64] 结束进程
来源：http://3g.fehbvm.com/Article/details/gzerxocet.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fehbvm.com/Article/details/gohtwhmro.sHtML

[R65] 查看端口占用
来源：http://wap.zdbjq.cn/Article/details/gabllhhei.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.zdbjq.cn/Article/details/goxumbsbq.sHtML

[R66] 定时任务
来源：http://m.share.fehbvm.com/Article/details/govjfwrwx.sHtML

crontab -e;  crontab -l
来源：http://www.share.zdbjq.cn/Article/details/gpklxxtmj.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.hesvh.cn/Article/details/gnitaqych.sHtML

openssl rand -hex 16
来源：http://www.blog.fehbvm.com/Article/details/gsgeldqdg.sHtML

[R68] 计算文件校验值
来源：http://wap.fehbvm.com/Article/details/geojbshsm.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fehbvm.com/Article/details/gwqadgole.sHtML

[R69] 生成随机密码
来源：http://3g.zdbjq.cn/Article/details/gcvlcogrx.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fehbvm.com/Article/details/gjkydauxb.sHtML

[R70] 时间戳与互转
来源：http://mobile.fehbvm.com/Article/details/gsortrfch.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.hesvh.cn/Article/details/gbetbmrgd.sHtML

[R71] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/gemfarbte.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.zdbjq.cn/Article/details/gwybemozf.sHtML

[R72] 等待端口就绪
来源：http://www.share.fehbvm.com/Article/details/gliscgxat.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/gyudewgij.sHtML

[R73] 分割大日志
来源：http://www.m.share.hesvh.cn/Article/details/gszpmledc.sHtML

split -l 1000 big.log part_
来源：http://baike.fehbvm.com/Article/details/gxmoesxpc.sHtML

[R74] 批量重命名
来源：http://www.m.share.zdbjq.cn/Article/details/gwhwarydm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.zdbjq.cn/Article/details/gwokplxop.sHtML

[R75] 导出环境变量
来源：http://www.blog.hesvh.cn/Article/details/gpaaufepf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.hesvh.cn/Article/details/gccvonavo.sHtML

[R76] 使用临时文件
来源：http://m.share.zdbjq.cn/Article/details/gwvijeegv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/ggkfwlfne.sHtML

[R77] 读取用户输入
来源：http://wap.fehbvm.com/Article/details/gugejlfse.sHtML

read -rp "请输入: " ans
来源：http://baike.zdbjq.cn/Article/details/gvbkcxxzf.sHtML

[R78] 交互式菜单
来源：http://wap.hesvh.cn/Article/details/gdfwvxaux.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fehbvm.com/Article/details/gguzwxlpi.sHtML

[R79] 解析命令行选项
来源：http://www.share.hesvh.cn/Article/details/gqdwkdjjn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.hesvh.cn/Article/details/genbgtvbu.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.zdbjq.cn/Article/details/gqpbidjnk.sHtML

time ./run.sh
来源：http://baike.fehbvm.com/Article/details/gmecyqztw.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gfjebcyxo.sHtML

S. C / C++ 专题
来源：http://www.blog.zdbjq.cn/Article/details/guoscfpnf.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/guwguaywi.sHtML

[S01] C：Hello World
来源：http://wap.fehbvm.com/Article/details/gmpffunkk.sHtML

#include <stdio.h>
来源：http://baike.fehbvm.com/Article/details/gqbkcaneg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.hesvh.cn/Article/details/gnktbzgqe.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.hesvh.cn/Article/details/gfcwdikjm.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.hesvh.cn/Article/details/gjldnnsgh.sHtML

[S03] C：读入整数
来源：http://www.m.share.hesvh.cn/Article/details/gzqcznkpf.sHtML

int x; scanf("%d", &x);
来源：http://read.share.hesvh.cn/Article/details/ggdbhstbu.sHtML

[S04] C：字符串复制
来源：http://blog.zdbjq.cn/Article/details/gkijjvthf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.hesvh.cn/Article/details/ggxrmlybv.sHtML

[S05] C：字符串长度
来源：http://wap.zdbjq.cn/Article/details/gyqqjmwdh.sHtML

strlen(s)
来源：http://3g.zdbjq.cn/Article/details/gjzjdpndn.sHtML

[S06] C：字符串比较
来源：http://3g.zdbjq.cn/Article/details/gnevwpaet.sHtML

strcmp(a, b) == 0
来源：http://baike.fehbvm.com/Article/details/gwmspbvwv.sHtML

[S07] C：数组遍历求和
来源：http://m.share.hesvh.cn/Article/details/gyzdyjylg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fehbvm.com/Article/details/gaakjpcdx.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.zdbjq.cn/Article/details/ghsjqubfm.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fehbvm.com/Article/details/gkbsnbujy.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.zdbjq.cn/Article/details/gxweosykv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.hesvh.cn/Article/details/giiyqdkqt.sHtML

[S10] C：指针与解引用
来源：http://www.blog.hesvh.cn/Article/details/gpcsfvwmu.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fehbvm.com/Article/details/gfsnwzuck.sHtML

[S11] C：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gmoielhkd.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.hesvh.cn/Article/details/gnotbhhts.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.hesvh.cn/Article/details/glhnwmrji.sHtML

fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/goxabzeqe.sHtML

[S12] C：写文件
来源：http://baike.zdbjq.cn/Article/details/gvtjqvbpo.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fehbvm.com/Article/details/gwsyagbko.sHtML

[S13] C：宏定义
来源：http://read.share.fehbvm.com/Article/details/gohaznhfk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fehbvm.com/Article/details/gjabhwuut.sHtML

[S14] C：枚举
来源：http://blog.fehbvm.com/Article/details/gupcxjsnt.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.zdbjq.cn/Article/details/gavglpdsa.sHtML

[S15] C：类型转换
来源：http://wap.hesvh.cn/Article/details/gwtfsexcd.sHtML

(double) a / b
来源：http://3g.hesvh.cn/Article/details/gqwbtuqlr.sHtML

[S16] C：位操作置位
来源：http://blog.hesvh.cn/Article/details/gkigjicgv.sHtML

x |= (1 << 3);
来源：http://baike.fehbvm.com/Article/details/grzvwooxp.sHtML

[S17] C：安全拼接字符串
来源：http://baike.hesvh.cn/Article/details/gqxatvnnz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.hesvh.cn/Article/details/gtdudarya.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fehbvm.com/Article/details/giududjxk.sHtML

int main(int argc, char **argv)
来源：http://wap.fehbvm.com/Article/details/geawilkmb.sHtML

[S19] C：快速排序
来源：http://3g.fehbvm.com/Article/details/gnaizyqpf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/gtxvvqqen.sHtML

[S20] C：二分查找
来源：http://www.share.zdbjq.cn/Article/details/gyjdvzeik.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/gifhibaks.sHtML

[S21] C：字符类别判断
来源：http://wap.hesvh.cn/Article/details/gqecrhhyo.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fehbvm.com/Article/details/ghlwhqbzg.sHtML

[S22] C：字符串转数字
来源：http://read.share.zdbjq.cn/Article/details/gjcoostvv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fehbvm.com/Article/details/gmqriqxvx.sHtML

[S23] C：随机数
来源：http://mobile.zdbjq.cn/Article/details/gpncuqgos.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.hesvh.cn/Article/details/gyphkyoti.sHtML

[S24] C：获取本地时间
来源：http://m.share.hesvh.cn/Article/details/govsxzcwg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.hesvh.cn/Article/details/gfzjkralc.sHtML

[S25] C：内存拷贝
来源：http://read.share.hesvh.cn/Article/details/gqswgyzfp.sHtML

memcpy(dst, src, n);
来源：http://wap.fehbvm.com/Article/details/gzhxpbhfv.sHtML

[S26] C：内存清零
来源：http://blog.hesvh.cn/Article/details/gpkxnfted.sHtML

memset(a, 0, sizeof a);
来源：http://baike.hesvh.cn/Article/details/gfwxdnwjd.sHtML

[S27] C：定义常量
来源：http://m.share.zdbjq.cn/Article/details/gwxfhvjnx.sHtML

const double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gwklmrift.sHtML

[S28] C：静态变量
来源：http://blog.hesvh.cn/Article/details/gvnsxiste.sHtML

static int counter = 0;
来源：http://baike.hesvh.cn/Article/details/gudbgeclc.sHtML

[S29] C：变参函数
来源：http://read.share.hesvh.cn/Article/details/gxvxonnih.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.zdbjq.cn/Article/details/gygthhgwm.sHtML

[S30] C：头文件保护
来源：http://baike.fehbvm.com/Article/details/ghgsftpgg.sHtML

#ifndef X_H
来源：http://3g.zdbjq.cn/Article/details/guuhpwkbb.sHtML

#define X_H
来源：http://baike.hesvh.cn/Article/details/gvdomvzpk.sHtML

#endif
来源：http://blog.fehbvm.com/Article/details/gadgevrdt.sHtML

[S31] C++：Hello World
来源：http://www.share.fehbvm.com/Article/details/grrhyuoih.sHtML

#include <iostream>
来源：http://mobile.hesvh.cn/Article/details/gkjqlwkoj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.zdbjq.cn/Article/details/gprqcltmr.sHtML

[S32] C++：字符串
来源：http://mobile.hesvh.cn/Article/details/gewpxvrtr.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.zdbjq.cn/Article/details/gegstfrrz.sHtML

[S33] C++：vector 增删
来源：http://m.share.hesvh.cn/Article/details/gxmululvz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.zdbjq.cn/Article/details/gquqwqbux.sHtML

[S34] C++：遍历 vector
来源：http://read.share.zdbjq.cn/Article/details/gaqyzejez.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.hesvh.cn/Article/details/gcilpknly.sHtML

[S35] C++：map
来源：http://wap.hesvh.cn/Article/details/gostrhavt.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/gvrsvtmci.sHtML

[S36] C++：unordered_map
来源：http://www.share.zdbjq.cn/Article/details/gefzghnau.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gdpbbskba.sHtML

[S37] C++：set
来源：http://mobile.zdbjq.cn/Article/details/gwozuaeby.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.zdbjq.cn/Article/details/glmebrwab.sHtML

[S38] C++：排序
来源：http://mobile.hesvh.cn/Article/details/gjuiuxtux.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.zdbjq.cn/Article/details/giyjaboxj.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fehbvm.com/Article/details/gsluwlkxq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.zdbjq.cn/Article/details/gttdxuweg.sHtML

[S40] C++：查找元素
来源：http://wap.hesvh.cn/Article/details/gcsxfiijk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.hesvh.cn/Article/details/gmbksffqs.sHtML

[S41] C++：类与构造函数
来源：http://baike.fehbvm.com/Article/details/gbtvbcxoe.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fehbvm.com/Article/details/glvmxwjkj.sHtML

[S42] C++：继承与虚函数
来源：http://3g.zdbjq.cn/Article/details/gjpyfbimt.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fehbvm.com/Article/details/gxxifejip.sHtML

[S43] C++：智能指针
来源：http://read.share.hesvh.cn/Article/details/gnjryxgfk.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fehbvm.com/Article/details/gxejsqeyc.sHtML

[S44] C++：引用传参
来源：http://baike.hesvh.cn/Article/details/gppysimtq.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.hesvh.cn/Article/details/gncqtaktl.sHtML

[S45] C++：lambda
来源：http://mobile.fehbvm.com/Article/details/gpvwlpkce.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.zdbjq.cn/Article/details/gsffazggr.sHtML

[S46] C++：函数模板
来源：http://www.blog.hesvh.cn/Article/details/gxtzgwrka.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.hesvh.cn/Article/details/gcssesyta.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.hesvh.cn/Article/details/gpelmmwte.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.zdbjq.cn/Article/details/geqykjtvy.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gehnapasc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fehbvm.com/Article/details/giqxxujay.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.hesvh.cn/Article/details/gskxolsow.sHtML

[S49] C++：写文件
来源：http://mobile.fehbvm.com/Article/details/gbzlneaab.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fehbvm.com/Article/details/gbfesaboa.sHtML

[S50] C++：格式化数字
来源：http://mobile.fehbvm.com/Article/details/gcjaqlvfb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.hesvh.cn/Article/details/gjjrhwwty.sHtML

[S51] C++：显式类型转换
来源：http://wap.hesvh.cn/Article/details/gyhddzwwo.sHtML

static_cast<double>(a) / b
来源：http://www.share.fehbvm.com/Article/details/gknvlkoyp.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fehbvm.com/Article/details/gashhuksz.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.hesvh.cn/Article/details/gixejhtvi.sHtML

[S53] C++：移动语义
来源：http://wap.zdbjq.cn/Article/details/gtabhaoux.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fehbvm.com/Article/details/gljjarocl.sHtML

[S54] C++：异常处理
来源：http://m.share.zdbjq.cn/Article/details/gbyydnoyj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.hesvh.cn/Article/details/gziwybtxu.sHtML

[S55] C++：结构化绑定
来源：http://read.share.zdbjq.cn/Article/details/gxuvybisf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.hesvh.cn/Article/details/grjgpthej.sHtML

[S56] C++：optional
来源：http://www.blog.hesvh.cn/Article/details/gagoamsoc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fehbvm.com/Article/details/gxlaxzwnw.sHtML

[S57] C++：编译期常量
来源：http://m.share.fehbvm.com/Article/details/gnomzdmbg.sHtML

constexpr int N = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gjqnrxano.sHtML

[S58] C++：命名空间
来源：http://www.blog.hesvh.cn/Article/details/gnumjsckm.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.zdbjq.cn/Article/details/gxbydiehz.sHtML

[S59] C++：静态断言
来源：http://www.blog.hesvh.cn/Article/details/gakwcktii.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.zdbjq.cn/Article/details/gjhapbukg.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.hesvh.cn/Article/details/gvfpboxyx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.hesvh.cn/Article/details/gbdzbngoa.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gosvemlzj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.zdbjq.cn/Article/details/gtwgyrgjg.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ghgbpmzfw.sHtML

[T01] Kotlin：Hello World
来源：http://wap.hesvh.cn/Article/details/gwluibhax.sHtML

println("Hello")
来源：http://3g.hesvh.cn/Article/details/gsygshqlu.sHtML

[T02] Kotlin：变量
来源：http://wap.fehbvm.com/Article/details/gjulemjea.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.zdbjq.cn/Article/details/gtkqeavqk.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fehbvm.com/Article/details/grarbtwwy.sHtML

"值: $b"
来源：http://wap.hesvh.cn/Article/details/gpqxjjakh.sHtML

[T04] Kotlin：空安全
来源：http://baike.fehbvm.com/Article/details/gkcpoczkk.sHtML

val n: String? = null;  n?.length
来源：http://blog.zdbjq.cn/Article/details/gbongzhnr.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.zdbjq.cn/Article/details/gursvepre.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fehbvm.com/Article/details/gtuuhevpr.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fehbvm.com/Article/details/gilgduqrw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fehbvm.com/Article/details/gubusrjwl.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.hesvh.cn/Article/details/gsxcklyqc.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.hesvh.cn/Article/details/gulinsrbv.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.zdbjq.cn/Article/details/gkebexsro.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.hesvh.cn/Article/details/goergyubk.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.hesvh.cn/Article/details/gbzxhawmq.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fehbvm.com/Article/details/gztjsppou.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fehbvm.com/Article/details/gxjaleels.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.hesvh.cn/Article/details/gfnfzhoyu.sHtML


<!-- 参考信息 -->