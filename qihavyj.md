代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gciejepce.sHtML

[R16] until 等待条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gytxthrew.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqhqrebl.sHtML

[R17] 数组定义与取值
来源：http://baike.fanxiaobao.xyz/Article/details/gmncojwyr.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grkoacvlc.sHtML

[R18] 遍历数组
来源：http://mobile.fanxiaobao.xyz/Article/details/gumqfhipv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/ggrzilolr.sHtML

[R19] 数组长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcilinmok.sHtML

echo "${#arr[@]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gxrntyoxt.sHtML

[R20] 关联数组（字典）
来源：http://wap.fanxiaobao.xyz/Article/details/grvtbirtk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyfajrjbb.sHtML

[R21] 字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gazgoeedz.sHtML

echo "${#s}"
来源：http://wap.fanxiaobao.xyz/Article/details/gjqufrzjt.sHtML

[R22] 截取子串
来源：http://3g.fanxiaobao.xyz/Article/details/gxfbgurno.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gebxcngyv.sHtML

[R23] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gnnqqctap.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fanxiaobao.xyz/Article/details/giivaaluv.sHtML

[R24] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gguabylrl.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fanxiaobao.xyz/Article/details/ghrqrpgvr.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsqzawvck.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gclibyhnt.sHtML

[R26] 命令替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gefawarla.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnemchqnc.sHtML

[R27] 算术展开
来源：http://m.share.fanxiaobao.xyz/Article/details/ggftolehj.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fanxiaobao.xyz/Article/details/garnnkhez.sHtML

[R28] 浮点运算
来源：http://m.share.fanxiaobao.xyz/Article/details/gzanbkbfe.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fanxiaobao.xyz/Article/details/gdxoznbiy.sHtML

[R29] 定义函数
来源：http://3g.fanxiaobao.xyz/Article/details/gfoogqlqh.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fanxiaobao.xyz/Article/details/gxnxphrje.sHtML

[R30] 函数返回状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/ghytcvozx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fanxiaobao.xyz/Article/details/gngourpvu.sHtML

[R31] 局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/ghpvuwaor.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/grkkgiwaz.sHtML

[R32] 参数个数校验
来源：http://read.share.fanxiaobao.xyz/Article/details/gkmhvtspg.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gnibmliyq.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqlxbjtb.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fanxiaobao.xyz/Article/details/gthvpmffq.sHtML

[R34] 退出时清理
来源：http://www.share.fanxiaobao.xyz/Article/details/giadfqmvq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzgwncizr.sHtML

[R35] 后台执行并等待
来源：http://mobile.fanxiaobao.xyz/Article/details/gerzaaknb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fanxiaobao.xyz/Article/details/gcvszeijh.sHtML

[R36] 并发执行多个任务
来源：http://blog.fanxiaobao.xyz/Article/details/gcdzjxqev.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fanxiaobao.xyz/Article/details/gtexwkahu.sHtML

[R37] 把输出赋给变量
来源：http://3g.fanxiaobao.xyz/Article/details/gkijquncl.sHtML

files=$(ls -1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvdtbgcid.sHtML

[R38] 管道串联
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxwzvyqbz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fanxiaobao.xyz/Article/details/gvjxrdcrm.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gidgjwpbh.sHtML

cmd > out.log 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gcwbhrehj.sHtML

[R40] 追加写日志
来源：http://baike.fanxiaobao.xyz/Article/details/gdzabmajt.sHtML

echo "log" >> out.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gkpnkfynw.sHtML

[R41] 丢弃输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gqgsdubdq.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gfaqskhnx.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/gcgtfutsp.sHtML

wc -l < a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gsuupkfem.sHtML

[R43] 按名字查找文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gbmcngeuo.sHtML

find . -name "*.log" -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gksufnuvu.sHtML

[R44] 按修改时间查找
来源：http://blog.fanxiaobao.xyz/Article/details/gkvbjmknj.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gybhnvmdh.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/gxjdhtsqg.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fanxiaobao.xyz/Article/details/gcgbwdzua.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fanxiaobao.xyz/Article/details/grqkwllkp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fanxiaobao.xyz/Article/details/gdurqlrol.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/glrakwpkx.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqxphuxz.sHtML

[R48] awk 取指定列
来源：http://www.share.fanxiaobao.xyz/Article/details/gedevwavy.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/guqfktyzi.sHtML

[R49] awk 带条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/glaviwqea.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqbrlrly.sHtML

[R50] awk 求和
来源：http://baike.fanxiaobao.xyz/Article/details/ggjakbrnc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqshehems.sHtML

[R51] 排序去重取前几
来源：http://3g.fanxiaobao.xyz/Article/details/goqcxhaqd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fanxiaobao.xyz/Article/details/gcquelhem.sHtML

[R52] 统计行数
来源：http://wap.fanxiaobao.xyz/Article/details/gmjtnlyyk.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gjqpbnwkf.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fanxiaobao.xyz/Article/details/gdocapjhf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fanxiaobao.xyz/Article/details/geelhdprn.sHtML

[R54] 比较两个文件
来源：http://baike.fanxiaobao.xyz/Article/details/ghqwinfep.sHtML

diff a.txt b.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gyhzbuycd.sHtML

[R55] 压缩与解压
来源：http://wap.fanxiaobao.xyz/Article/details/gqxxrqhvz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fanxiaobao.xyz/Article/details/ggperbytc.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gjujmfxlh.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/gnopqvghp.sHtML

[R57] 远程执行命令
来源：http://m.share.fanxiaobao.xyz/Article/details/gnhuikaux.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxebblkwv.sHtML

[R58] 下载文件
来源：http://baike.fanxiaobao.xyz/Article/details/gzmazcgnh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fanxiaobao.xyz/Article/details/gwookuqbn.sHtML

[R59] 发 POST JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gtencznpn.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/gojkosaec.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gaxiyitsu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fanxiaobao.xyz/Article/details/gnfvtxawz.sHtML

[R61] 磁盘占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbguwzuqv.sHtML

df -h;  du -sh *
来源：http://blog.fanxiaobao.xyz/Article/details/gykngfbqp.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/ggicluubd.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fanxiaobao.xyz/Article/details/gnumpsomh.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gizfdzcqk.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmnunnuqm.sHtML

[R64] 结束进程
来源：http://blog.fanxiaobao.xyz/Article/details/giqtahrtm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fanxiaobao.xyz/Article/details/gewvbhypi.sHtML

[R65] 查看端口占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gunxfbviz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fanxiaobao.xyz/Article/details/ghbrmeffd.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gkyfewnjk.sHtML

crontab -e;  crontab -l
来源：http://baike.fanxiaobao.xyz/Article/details/gpzwzjpct.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglaywggs.sHtML

openssl rand -hex 16
来源：http://blog.fanxiaobao.xyz/Article/details/ggwjzjozc.sHtML

[R68] 计算文件校验值
来源：http://m.share.fanxiaobao.xyz/Article/details/gioduyohj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gvesrthaw.sHtML

[R69] 生成随机密码
来源：http://blog.fanxiaobao.xyz/Article/details/gyyjnyqrd.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fanxiaobao.xyz/Article/details/gtfoihtcv.sHtML

[R70] 时间戳与互转
来源：http://blog.fanxiaobao.xyz/Article/details/gnrymnkri.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fanxiaobao.xyz/Article/details/gomuidfww.sHtML

[R71] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gtwyafldi.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fanxiaobao.xyz/Article/details/glqjmagst.sHtML

[R72] 等待端口就绪
来源：http://blog.fanxiaobao.xyz/Article/details/geiqigkwv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gldasbzpo.sHtML

[R73] 分割大日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gakzpywtl.sHtML

split -l 1000 big.log part_
来源：http://wap.fanxiaobao.xyz/Article/details/gxaiopndn.sHtML

[R74] 批量重命名
来源：http://3g.fanxiaobao.xyz/Article/details/goxgbvduu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gqzuxltib.sHtML

[R75] 导出环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwtohlunw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fanxiaobao.xyz/Article/details/gabalnnbq.sHtML

[R76] 使用临时文件
来源：http://wap.fanxiaobao.xyz/Article/details/gafcjuyqk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gsbtrwbwq.sHtML

[R77] 读取用户输入
来源：http://blog.fanxiaobao.xyz/Article/details/gsemmubul.sHtML

read -rp "请输入: " ans
来源：http://mobile.fanxiaobao.xyz/Article/details/gsygpnvlf.sHtML

[R78] 交互式菜单
来源：http://www.share.fanxiaobao.xyz/Article/details/gqwrwkcwe.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gfuejpltf.sHtML

[R79] 解析命令行选项
来源：http://m.share.fanxiaobao.xyz/Article/details/guodqavfi.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/guwbjemnm.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjofwjfh.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjuffsln.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjnqiiql.sHtML

S. C / C++ 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gzszimbvl.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/girvsaydo.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gtffzxytq.sHtML

#include <stdio.h>
来源：http://baike.fanxiaobao.xyz/Article/details/gvrfcxulz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpjatyqzn.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gxrqjqcvz.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/guvyiasrx.sHtML

[S03] C：读入整数
来源：http://wap.fanxiaobao.xyz/Article/details/geemacwjq.sHtML

int x; scanf("%d", &x);
来源：http://wap.fanxiaobao.xyz/Article/details/gwgkuualk.sHtML

[S04] C：字符串复制
来源：http://www.blog.fanxiaobao.xyz/Article/details/glhvgycom.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvojbdam.sHtML

[S05] C：字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gcxblousx.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gfthjbzhj.sHtML

[S06] C：字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gdfovkzoo.sHtML

strcmp(a, b) == 0
来源：http://blog.fanxiaobao.xyz/Article/details/gwnflhizm.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfbleyzp.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fanxiaobao.xyz/Article/details/girjwzzqp.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/glwicbklj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjeoohbf.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fanxiaobao.xyz/Article/details/gzufroprp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fanxiaobao.xyz/Article/details/gazowbkjg.sHtML

[S10] C：指针与解引用
来源：http://www.share.fanxiaobao.xyz/Article/details/gmmrpfgjo.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gvwgytfip.sHtML

[S11] C：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gzcyiywdd.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/gsyyonjnl.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/grdvdnmxb.sHtML

fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/giaaadjzn.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gdnguyjfn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghgqsdnyz.sHtML

[S13] C：宏定义
来源：http://blog.fanxiaobao.xyz/Article/details/gikcnbdgs.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbqyjbuo.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gwdcokmtd.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fanxiaobao.xyz/Article/details/gaohrhyhd.sHtML

[S15] C：类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gipotutdv.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/gdobgzmpy.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gotcbthap.sHtML

x |= (1 << 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gtsvpoeop.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gayszsavr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fanxiaobao.xyz/Article/details/gxtpepjaj.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gohvzpklu.sHtML

int main(int argc, char **argv)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwgqgwesd.sHtML

[S19] C：快速排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gkljosori.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gierxoviv.sHtML

[S20] C：二分查找
来源：http://wap.fanxiaobao.xyz/Article/details/giixrxirl.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbwkacgh.sHtML

[S21] C：字符类别判断
来源：http://3g.fanxiaobao.xyz/Article/details/gzfrdevpa.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fanxiaobao.xyz/Article/details/gcypiqxef.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/gonmlqytz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fanxiaobao.xyz/Article/details/gozppwuom.sHtML

[S23] C：随机数
来源：http://3g.fanxiaobao.xyz/Article/details/gyhkpwrky.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtspiolhx.sHtML

[S24] C：获取本地时间
来源：http://blog.fanxiaobao.xyz/Article/details/gqwjeegvb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fanxiaobao.xyz/Article/details/gensvsiie.sHtML

[S25] C：内存拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gxmlyqbut.sHtML

memcpy(dst, src, n);
来源：http://m.share.fanxiaobao.xyz/Article/details/grmxwwize.sHtML

[S26] C：内存清零
来源：http://wap.fanxiaobao.xyz/Article/details/gnonvgtpk.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gveydmbbu.sHtML

[S27] C：定义常量
来源：http://3g.fanxiaobao.xyz/Article/details/gplqqlsch.sHtML

const double PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gidmhrleq.sHtML

[S28] C：静态变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gwogrlhuv.sHtML

static int counter = 0;
来源：http://wap.fanxiaobao.xyz/Article/details/gxafmhzed.sHtML

[S29] C：变参函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gagtijfwz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmxtsglhd.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdolxgcgp.sHtML

#ifndef X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gdrkvjsku.sHtML

#define X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gsnkflhej.sHtML

#endif
来源：http://3g.fanxiaobao.xyz/Article/details/gixrhdnts.sHtML

[S31] C++：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gtwubufye.sHtML

#include <iostream>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvhkajeqk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjyfmkbai.sHtML

[S32] C++：字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gxvomxakw.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fanxiaobao.xyz/Article/details/ghfydwgjp.sHtML

[S33] C++：vector 增删
来源：http://wap.fanxiaobao.xyz/Article/details/gdnfddcct.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gokjpcuvi.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fanxiaobao.xyz/Article/details/gxsutyule.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/garqxjwim.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/gomusmwzp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gikryxbgy.sHtML

[S36] C++：unordered_map
来源：http://mobile.fanxiaobao.xyz/Article/details/geacwwagt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjyfwcfxn.sHtML

[S37] C++：set
来源：http://wap.fanxiaobao.xyz/Article/details/gvpvvhjlt.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gasiihizd.sHtML

[S38] C++：排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gfawagjay.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gakbyrqtz.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gzfzoypos.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fanxiaobao.xyz/Article/details/gacqtqydt.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gbifosowv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gbvfmfrmf.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fanxiaobao.xyz/Article/details/guczovynd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fanxiaobao.xyz/Article/details/gclznevrn.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gwodgvcyi.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/ggmvsuafm.sHtML

[S43] C++：智能指针
来源：http://3g.fanxiaobao.xyz/Article/details/gblrzubaq.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fanxiaobao.xyz/Article/details/ginthalrl.sHtML

[S44] C++：引用传参
来源：http://read.share.fanxiaobao.xyz/Article/details/gfpleajtu.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giehizqsi.sHtML

[S45] C++：lambda
来源：http://blog.fanxiaobao.xyz/Article/details/gduhfxgty.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fanxiaobao.xyz/Article/details/givltdutr.sHtML

[S46] C++：函数模板
来源：http://baike.fanxiaobao.xyz/Article/details/gkygkgipz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbkkvnrbz.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gkfdghxnm.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfimhzhbe.sHtML

[S48] C++：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gnzqljpzx.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqqwdfkvr.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxacbhclk.sHtML

[S49] C++：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gyzkfjjfh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gepnmnvty.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gorhsqqfa.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gsdiueggk.sHtML

[S51] C++：显式类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/glqekthbh.sHtML

static_cast<double>(a) / b
来源：http://baike.fanxiaobao.xyz/Article/details/gqxolrqrt.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fanxiaobao.xyz/Article/details/gfvljtwqs.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gufoptmky.sHtML

[S53] C++：移动语义
来源：http://mobile.fanxiaobao.xyz/Article/details/gxqkjqxez.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fanxiaobao.xyz/Article/details/gneuzvidi.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpcswtopa.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpoemqcoh.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqutxbugc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/gblylguqv.sHtML

[S56] C++：optional
来源：http://read.share.fanxiaobao.xyz/Article/details/glyhxdtea.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqzbilpje.sHtML

[S57] C++：编译期常量
来源：http://baike.fanxiaobao.xyz/Article/details/gxofpaprb.sHtML

constexpr int N = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gddvuxjjz.sHtML

[S58] C++：命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggwxgfbfr.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fanxiaobao.xyz/Article/details/gcfepjcky.sHtML

[S59] C++：静态断言
来源：http://m.share.fanxiaobao.xyz/Article/details/gjirmyfjm.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fanxiaobao.xyz/Article/details/gllueywpa.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gsecqraba.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gkuuovlga.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gmczjvspl.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fanxiaobao.xyz/Article/details/gacnrdxyi.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gbljpokev.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gyrcrbehs.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gexfoqzkw.sHtML

[T02] Kotlin：变量
来源：http://3g.fanxiaobao.xyz/Article/details/gcajxvgtf.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fanxiaobao.xyz/Article/details/gehkbtyjs.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fanxiaobao.xyz/Article/details/gerqcfyxl.sHtML

"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/godqcuhec.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqrranfpp.sHtML

val n: String? = null;  n?.length
来源：http://3g.fanxiaobao.xyz/Article/details/gxcfqflhs.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gezwzkjzw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fanxiaobao.xyz/Article/details/gtxgqxdhz.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/gxyyhxljd.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/groaworbw.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gsukygbwb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhoxnwxe.sHtML

[T08] Kotlin：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/gqtxzljbe.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/gfcztylvi.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gjjrzungo.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fanxiaobao.xyz/Article/details/gwfbdeeyx.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fanxiaobao.xyz/Article/details/gfbcvoqnq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fanxiaobao.xyz/Article/details/gvxznybwo.sHtML

[T11] Kotlin：协程
来源：http://m.share.fanxiaobao.xyz/Article/details/gfhykflml.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwwnvrchw.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fanxiaobao.xyz/Article/details/gykshbifl.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcrozcavs.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/grrcygccq.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gooyjumhr.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyjbyqskg.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxklkanwx.sHtML

[T15] Kotlin：接口
来源：http://read.share.fanxiaobao.xyz/Article/details/gyhdxrffu.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqcisdjn.sHtML

[T16] Swift：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gwsvvsrea.sHtML

print("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gerqhwdyg.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grenseywd.sHtML

var a = 1;  let b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gifiztbaq.sHtML

[T18] Swift：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gayktwive.sHtML

"值: \(b)"
来源：http://3g.fanxiaobao.xyz/Article/details/gueadkrgt.sHtML


<!-- 参考信息 -->