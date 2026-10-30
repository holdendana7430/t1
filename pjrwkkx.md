代发 wailian999

case "$1" in
来源：http://3g.hesvh.cn/Article/details/gbypvhfkw.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gwivodgqj.sHtML

stop)  echo "停止" ;;
来源：http://3g.fehbvm.com/Article/details/gbqfvlilj.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fehbvm.com/Article/details/gotpoalop.sHtML

esac
来源：http://www.share.zdbjq.cn/Article/details/gbfywgyhg.sHtML

[R12] for 遍历文件
来源：http://mobile.zdbjq.cn/Article/details/gntuciqvj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.hesvh.cn/Article/details/gxtncacsa.sHtML

[R13] for 计数循环
来源：http://baike.hesvh.cn/Article/details/gvhrmpbmp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/gndphtkqn.sHtML

[R14] C 风格 for
来源：http://3g.hesvh.cn/Article/details/gwkdvpzkj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/gzgyxgcxa.sHtML

[R15] while 逐行读文件
来源：http://blog.fehbvm.com/Article/details/gasdtcyht.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.hesvh.cn/Article/details/gkzclhvvx.sHtML

[R16] until 等待条件
来源：http://m.share.zdbjq.cn/Article/details/geqayqhtl.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gwzkqixoz.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fehbvm.com/Article/details/gpvxxxnhx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gxylkaite.sHtML

[R18] 遍历数组
来源：http://www.m.share.hesvh.cn/Article/details/gvezhbrky.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.zdbjq.cn/Article/details/gxgyeqiki.sHtML

[R19] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/gujqdkspd.sHtML

echo "${#arr[@]}"
来源：http://mobile.fehbvm.com/Article/details/gdvnslhkk.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.zdbjq.cn/Article/details/ggteyfcsd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fehbvm.com/Article/details/gecsesrek.sHtML

[R21] 字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gqmydvyxz.sHtML

echo "${#s}"
来源：http://mobile.fehbvm.com/Article/details/gcnagwfjn.sHtML

[R22] 截取子串
来源：http://wap.zdbjq.cn/Article/details/gkdqxylab.sHtML

echo "${s:0:5}"
来源：http://www.blog.zdbjq.cn/Article/details/gcaugosov.sHtML

[R23] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/ggbjtvtou.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.hesvh.cn/Article/details/gzeopcxtw.sHtML

[R24] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gqjgfdxep.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fehbvm.com/Article/details/guukezizv.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.hesvh.cn/Article/details/gbnnzdnpm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.zdbjq.cn/Article/details/gkqnkoxnu.sHtML

[R26] 命令替换
来源：http://baike.hesvh.cn/Article/details/giktmacrc.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.hesvh.cn/Article/details/gbxxvfdjt.sHtML

[R27] 算术展开
来源：http://m.share.fehbvm.com/Article/details/gzrabunzd.sHtML

echo $((1 + 2 * 3))
来源：http://3g.hesvh.cn/Article/details/gtcdzkpex.sHtML

[R28] 浮点运算
来源：http://read.share.zdbjq.cn/Article/details/gxhikotcr.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fehbvm.com/Article/details/gwljkwfmd.sHtML

[R29] 定义函数
来源：http://m.share.fehbvm.com/Article/details/ghkfahzvy.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fehbvm.com/Article/details/gcqngqjie.sHtML

[R30] 函数返回状态码
来源：http://mobile.zdbjq.cn/Article/details/gidjvabfb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.zdbjq.cn/Article/details/gunmwsyxx.sHtML

[R31] 局部变量
来源：http://www.share.fehbvm.com/Article/details/ghcmnblfs.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.hesvh.cn/Article/details/guzoruwvv.sHtML

[R32] 参数个数校验
来源：http://3g.fehbvm.com/Article/details/gmccbfary.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gijkzjxkc.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.hesvh.cn/Article/details/ggnspdtzf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.zdbjq.cn/Article/details/gygvvywvf.sHtML

[R34] 退出时清理
来源：http://3g.zdbjq.cn/Article/details/gckxkulrp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/gowsyrtzt.sHtML

[R35] 后台执行并等待
来源：http://3g.zdbjq.cn/Article/details/gsjeivezy.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fehbvm.com/Article/details/ghspvsigq.sHtML

[R36] 并发执行多个任务
来源：http://baike.fehbvm.com/Article/details/gruplroxf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.zdbjq.cn/Article/details/gudifxxra.sHtML

[R37] 把输出赋给变量
来源：http://baike.fehbvm.com/Article/details/gtzqnqfwu.sHtML

files=$(ls -1)
来源：http://www.blog.zdbjq.cn/Article/details/gprcqfgec.sHtML

[R38] 管道串联
来源：http://read.share.fehbvm.com/Article/details/geegwlwli.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fehbvm.com/Article/details/gygvnrjml.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.zdbjq.cn/Article/details/ghvwjrqkg.sHtML

cmd > out.log 2>&1
来源：http://www.share.fehbvm.com/Article/details/gvzkxeled.sHtML

[R40] 追加写日志
来源：http://mobile.fehbvm.com/Article/details/gugdkmyne.sHtML

echo "log" >> out.log
来源：http://baike.zdbjq.cn/Article/details/gdmzsahna.sHtML

[R41] 丢弃输出
来源：http://read.share.hesvh.cn/Article/details/gpfcmljjr.sHtML

cmd >/dev/null 2>&1
来源：http://3g.zdbjq.cn/Article/details/gqwfopwxu.sHtML

[R42] 输入重定向
来源：http://www.blog.hesvh.cn/Article/details/gqsfdeojg.sHtML

wc -l < a.txt
来源：http://blog.hesvh.cn/Article/details/gyihbqvfr.sHtML

[R43] 按名字查找文件
来源：http://mobile.fehbvm.com/Article/details/gwnhkusfh.sHtML

find . -name "*.log" -type f
来源：http://www.blog.zdbjq.cn/Article/details/gtmxlifhd.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.hesvh.cn/Article/details/gxhkohdzs.sHtML

find . -mtime -7 -type f
来源：http://3g.hesvh.cn/Article/details/gsozokxet.sHtML

[R45] 批量删除
来源：http://mobile.zdbjq.cn/Article/details/gjqrqocyy.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.hesvh.cn/Article/details/gllleammm.sHtML

[R46] 递归替换文件内容
来源：http://wap.zdbjq.cn/Article/details/gacqexnye.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.zdbjq.cn/Article/details/gtzydhbag.sHtML

[R47] sed 单行替换
来源：http://blog.zdbjq.cn/Article/details/ggkrclvia.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gakftwgnh.sHtML

[R48] awk 取指定列
来源：http://www.share.zdbjq.cn/Article/details/gwpdkroiw.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/ggsxmzyot.sHtML

[R49] awk 带条件
来源：http://mobile.hesvh.cn/Article/details/gwskoaonl.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fehbvm.com/Article/details/gmzqbhjac.sHtML

[R50] awk 求和
来源：http://3g.zdbjq.cn/Article/details/gjqfftzjy.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gzlksssrq.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fehbvm.com/Article/details/grjyceaas.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.hesvh.cn/Article/details/gfyzlorbr.sHtML

[R52] 统计行数
来源：http://www.share.zdbjq.cn/Article/details/gmqcgnfzk.sHtML

wc -l a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gmvvnbsxo.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fehbvm.com/Article/details/gclxsnsyk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fehbvm.com/Article/details/gmqlbmzfj.sHtML

[R54] 比较两个文件
来源：http://wap.hesvh.cn/Article/details/gizbgjrek.sHtML

diff a.txt b.txt
来源：http://read.share.fehbvm.com/Article/details/gwoikhhej.sHtML

[R55] 压缩与解压
来源：http://www.blog.hesvh.cn/Article/details/gcjpdzdih.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.zdbjq.cn/Article/details/golvkrrmu.sHtML

[R56] 远程拷贝
来源：http://www.share.zdbjq.cn/Article/details/gxojjdfyi.sHtML

scp file user@host:/path/
来源：http://read.share.fehbvm.com/Article/details/glavpofib.sHtML

[R57] 远程执行命令
来源：http://www.blog.fehbvm.com/Article/details/gqmtaqczp.sHtML

ssh user@host 'uptime'
来源：http://read.share.zdbjq.cn/Article/details/gljijiysj.sHtML

[R58] 下载文件
来源：http://baike.hesvh.cn/Article/details/gaxcxoydz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.hesvh.cn/Article/details/gpypafedm.sHtML

[R59] 发 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/ggtpkcwnp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.hesvh.cn/Article/details/gskajulfb.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/gbfxhawty.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fehbvm.com/Article/details/gkfcmbvlx.sHtML

[R61] 磁盘占用
来源：http://blog.zdbjq.cn/Article/details/gnhvsxork.sHtML

df -h;  du -sh *
来源：http://www.m.share.zdbjq.cn/Article/details/gwufhanso.sHtML

[R62] 找最占空间的文件
来源：http://mobile.zdbjq.cn/Article/details/gnjuhijyv.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.zdbjq.cn/Article/details/gfqgjrzzy.sHtML

[R63] 内存与进程
来源：http://baike.hesvh.cn/Article/details/gppcdpkuc.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.zdbjq.cn/Article/details/govhpnspw.sHtML

[R64] 结束进程
来源：http://m.share.fehbvm.com/Article/details/gqdwvdqgc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.hesvh.cn/Article/details/grflkqlsw.sHtML

[R65] 查看端口占用
来源：http://read.share.fehbvm.com/Article/details/gexxtyedv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fehbvm.com/Article/details/guemhtpnk.sHtML

[R66] 定时任务
来源：http://3g.zdbjq.cn/Article/details/gefrfpahy.sHtML

crontab -e;  crontab -l
来源：http://www.blog.zdbjq.cn/Article/details/gukxoclkd.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.zdbjq.cn/Article/details/goyqbgtqt.sHtML

openssl rand -hex 16
来源：http://baike.hesvh.cn/Article/details/gujjxuono.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.zdbjq.cn/Article/details/gmmehjhxg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fehbvm.com/Article/details/gywpmxcpl.sHtML

[R69] 生成随机密码
来源：http://3g.hesvh.cn/Article/details/gxpkkqwnb.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fehbvm.com/Article/details/gwsgabmqd.sHtML

[R70] 时间戳与互转
来源：http://mobile.zdbjq.cn/Article/details/gwnkzzihz.sHtML

date +%s;  date -d @1700000000
来源：http://wap.hesvh.cn/Article/details/gvkygcbri.sHtML

[R71] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/gnztlahkr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fehbvm.com/Article/details/gckychasa.sHtML

[R72] 等待端口就绪
来源：http://m.share.hesvh.cn/Article/details/ggxdknjea.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/gudnusvxh.sHtML

[R73] 分割大日志
来源：http://read.share.zdbjq.cn/Article/details/gblkrwfmf.sHtML

split -l 1000 big.log part_
来源：http://blog.zdbjq.cn/Article/details/gqayafped.sHtML

[R74] 批量重命名
来源：http://www.m.share.hesvh.cn/Article/details/gxakqilps.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fehbvm.com/Article/details/gepwptkyl.sHtML

[R75] 导出环境变量
来源：http://read.share.zdbjq.cn/Article/details/gsvkendux.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fehbvm.com/Article/details/gxxuumzvq.sHtML

[R76] 使用临时文件
来源：http://wap.zdbjq.cn/Article/details/gklfygfcl.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/gaxjvazxm.sHtML

[R77] 读取用户输入
来源：http://read.share.fehbvm.com/Article/details/gycgcpyib.sHtML

read -rp "请输入: " ans
来源：http://3g.hesvh.cn/Article/details/gtlmzpxka.sHtML

[R78] 交互式菜单
来源：http://mobile.hesvh.cn/Article/details/ghcobdnfc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.zdbjq.cn/Article/details/gvfxesllb.sHtML

[R79] 解析命令行选项
来源：http://www.blog.zdbjq.cn/Article/details/ghakuwmjr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.zdbjq.cn/Article/details/gwszjdgwy.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.hesvh.cn/Article/details/gattoeizq.sHtML

time ./run.sh
来源：http://baike.hesvh.cn/Article/details/gibhqnhda.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gsffgkhxi.sHtML

S. C / C++ 专题
来源：http://mobile.fehbvm.com/Article/details/gljwtyxfi.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gfshrrahp.sHtML

[S01] C：Hello World
来源：http://wap.zdbjq.cn/Article/details/gfoveqrmv.sHtML

#include <stdio.h>
来源：http://mobile.fehbvm.com/Article/details/glmvzomzk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fehbvm.com/Article/details/ggunihxgw.sHtML

[S02] C：变量与格式化输出
来源：http://baike.hesvh.cn/Article/details/gvphfmcqo.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fehbvm.com/Article/details/gphgkamxx.sHtML

[S03] C：读入整数
来源：http://www.blog.hesvh.cn/Article/details/gtiqghrnx.sHtML

int x; scanf("%d", &x);
来源：http://m.share.zdbjq.cn/Article/details/gsacgqcxn.sHtML

[S04] C：字符串复制
来源：http://www.blog.hesvh.cn/Article/details/goindxxzb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.zdbjq.cn/Article/details/gkkdmulwl.sHtML

[S05] C：字符串长度
来源：http://m.share.fehbvm.com/Article/details/gnqutvuvo.sHtML

strlen(s)
来源：http://www.m.share.hesvh.cn/Article/details/gupjpeyyr.sHtML

[S06] C：字符串比较
来源：http://3g.fehbvm.com/Article/details/gozqftigd.sHtML

strcmp(a, b) == 0
来源：http://wap.fehbvm.com/Article/details/gyqtoucbh.sHtML

[S07] C：数组遍历求和
来源：http://wap.zdbjq.cn/Article/details/gpbytwwdy.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.hesvh.cn/Article/details/gempsmwdi.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fehbvm.com/Article/details/gvxxsxwjg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.hesvh.cn/Article/details/gcohxhpkp.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.zdbjq.cn/Article/details/gjtkfhvns.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.hesvh.cn/Article/details/gywqvuunx.sHtML

[S10] C：指针与解引用
来源：http://www.share.zdbjq.cn/Article/details/grcxufyzr.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fehbvm.com/Article/details/gkxhmqmsv.sHtML

[S11] C：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/ghlhtetwi.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.hesvh.cn/Article/details/gtsihfqog.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fehbvm.com/Article/details/gvwclkapp.sHtML

fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/gzjmsozff.sHtML

[S12] C：写文件
来源：http://m.share.hesvh.cn/Article/details/gdflfipyy.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fehbvm.com/Article/details/gpiqvjvrh.sHtML

[S13] C：宏定义
来源：http://www.m.share.hesvh.cn/Article/details/gqrnipidy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.hesvh.cn/Article/details/gortwpyjx.sHtML

[S14] C：枚举
来源：http://baike.hesvh.cn/Article/details/gtabxhumu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.zdbjq.cn/Article/details/gncumskgz.sHtML

[S15] C：类型转换
来源：http://3g.hesvh.cn/Article/details/gcbiemioy.sHtML

(double) a / b
来源：http://www.share.fehbvm.com/Article/details/gmxzqcntd.sHtML

[S16] C：位操作置位
来源：http://m.share.fehbvm.com/Article/details/gvtkmyskt.sHtML

x |= (1 << 3);
来源：http://www.share.zdbjq.cn/Article/details/gnhbyuqcf.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gftcvecif.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fehbvm.com/Article/details/gpbgwjlku.sHtML

[S18] C：命令行参数
来源：http://3g.fehbvm.com/Article/details/gmfnbcwff.sHtML

int main(int argc, char **argv)
来源：http://3g.hesvh.cn/Article/details/gkcnruhtc.sHtML

[S19] C：快速排序
来源：http://wap.zdbjq.cn/Article/details/grblwgttg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/gjogtlrli.sHtML

[S20] C：二分查找
来源：http://www.m.share.hesvh.cn/Article/details/gqchgauxt.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/gjhzymtwh.sHtML

[S21] C：字符类别判断
来源：http://wap.hesvh.cn/Article/details/gbkugfits.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fehbvm.com/Article/details/gwytkhjsr.sHtML

[S22] C：字符串转数字
来源：http://mobile.hesvh.cn/Article/details/gvwunralg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.hesvh.cn/Article/details/gexfgjliz.sHtML

[S23] C：随机数
来源：http://baike.fehbvm.com/Article/details/gxifbwtvu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.hesvh.cn/Article/details/gdpjrnyxh.sHtML

[S24] C：获取本地时间
来源：http://3g.hesvh.cn/Article/details/gewgknlet.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fehbvm.com/Article/details/gqdowcomd.sHtML

[S25] C：内存拷贝
来源：http://baike.hesvh.cn/Article/details/gtkoudpod.sHtML

memcpy(dst, src, n);
来源：http://wap.zdbjq.cn/Article/details/gkgjsozbp.sHtML

[S26] C：内存清零
来源：http://3g.hesvh.cn/Article/details/gljbxgddu.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.hesvh.cn/Article/details/gzqjtatzn.sHtML

[S27] C：定义常量
来源：http://wap.fehbvm.com/Article/details/gtcvcfada.sHtML

const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/grleferfa.sHtML

[S28] C：静态变量
来源：http://baike.hesvh.cn/Article/details/gqqguyaqg.sHtML

static int counter = 0;
来源：http://3g.zdbjq.cn/Article/details/gkbwxbbhv.sHtML

[S29] C：变参函数
来源：http://wap.zdbjq.cn/Article/details/ghmjkiagp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.zdbjq.cn/Article/details/glghogggh.sHtML

[S30] C：头文件保护
来源：http://read.share.hesvh.cn/Article/details/geprujibq.sHtML

#ifndef X_H
来源：http://m.share.zdbjq.cn/Article/details/gehipdqxc.sHtML

#define X_H
来源：http://mobile.zdbjq.cn/Article/details/gduvfwtwg.sHtML

#endif
来源：http://m.share.zdbjq.cn/Article/details/gclpgxkbn.sHtML

[S31] C++：Hello World
来源：http://wap.hesvh.cn/Article/details/gxsstbobo.sHtML

#include <iostream>
来源：http://blog.fehbvm.com/Article/details/gazyjsnpd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fehbvm.com/Article/details/guamqoztx.sHtML

[S32] C++：字符串
来源：http://read.share.hesvh.cn/Article/details/gurhcsybm.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.zdbjq.cn/Article/details/gxjqlpskd.sHtML

[S33] C++：vector 增删
来源：http://www.share.fehbvm.com/Article/details/gepoxnicy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.zdbjq.cn/Article/details/grbyaikyv.sHtML

[S34] C++：遍历 vector
来源：http://blog.zdbjq.cn/Article/details/gogqgbfzx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.hesvh.cn/Article/details/githceojs.sHtML

[S35] C++：map
来源：http://www.m.share.zdbjq.cn/Article/details/gwtbhllkz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gknlbomir.sHtML

[S36] C++：unordered_map
来源：http://blog.fehbvm.com/Article/details/gyaifcefm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gxhhzfzwh.sHtML

[S37] C++：set
来源：http://mobile.zdbjq.cn/Article/details/gmoketlox.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.hesvh.cn/Article/details/grfgjyjrw.sHtML

[S38] C++：排序
来源：http://blog.zdbjq.cn/Article/details/gqjtlsehl.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fehbvm.com/Article/details/gmeahsyox.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.zdbjq.cn/Article/details/gnopwiiqd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fehbvm.com/Article/details/gqmzujepj.sHtML

[S40] C++：查找元素
来源：http://baike.zdbjq.cn/Article/details/gihsmgkty.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.hesvh.cn/Article/details/gpiygkgbz.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fehbvm.com/Article/details/gjrujciup.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.hesvh.cn/Article/details/gwthzpvfz.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.hesvh.cn/Article/details/gcsjecgrd.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.zdbjq.cn/Article/details/gpuvzzpxy.sHtML

[S43] C++：智能指针
来源：http://baike.hesvh.cn/Article/details/gshwvwlir.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.hesvh.cn/Article/details/gmqrxadvg.sHtML

[S44] C++：引用传参
来源：http://www.share.fehbvm.com/Article/details/gwnsugppo.sHtML

void inc(int &x) { ++x; }
来源：http://3g.zdbjq.cn/Article/details/gahzhfnoq.sHtML

[S45] C++：lambda
来源：http://m.share.zdbjq.cn/Article/details/grklcmjcl.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.zdbjq.cn/Article/details/gqdrgbbhf.sHtML

[S46] C++：函数模板
来源：http://m.share.hesvh.cn/Article/details/goevihbls.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.zdbjq.cn/Article/details/gdfnmmgph.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.hesvh.cn/Article/details/gxvnpketg.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fehbvm.com/Article/details/gjixxqffo.sHtML

[S48] C++：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gopmkbcbs.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.zdbjq.cn/Article/details/gcruqdozq.sHtML

while (std::getline(in, line)) { }
来源：http://3g.zdbjq.cn/Article/details/gdtnjdgfz.sHtML

[S49] C++：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gmehkbhaz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fehbvm.com/Article/details/grzyievyh.sHtML

[S50] C++：格式化数字
来源：http://mobile.zdbjq.cn/Article/details/gmzyzxpiu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.hesvh.cn/Article/details/ghginandf.sHtML

[S51] C++：显式类型转换
来源：http://mobile.zdbjq.cn/Article/details/gbumnkasu.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fehbvm.com/Article/details/gizamdvey.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.zdbjq.cn/Article/details/gblicyjjl.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fehbvm.com/Article/details/gfsyeqxub.sHtML

[S53] C++：移动语义
来源：http://www.m.share.zdbjq.cn/Article/details/gmjbztdvv.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.zdbjq.cn/Article/details/gayrzxcsm.sHtML

[S54] C++：异常处理
来源：http://read.share.zdbjq.cn/Article/details/gdtokhoua.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fehbvm.com/Article/details/ggpzptmpf.sHtML

[S55] C++：结构化绑定
来源：http://baike.zdbjq.cn/Article/details/gphritnfi.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.hesvh.cn/Article/details/glngehewu.sHtML

[S56] C++：optional
来源：http://m.share.fehbvm.com/Article/details/gcmuelndk.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.zdbjq.cn/Article/details/grxaqruzu.sHtML

[S57] C++：编译期常量
来源：http://wap.fehbvm.com/Article/details/ggibdhhwu.sHtML

constexpr int N = 10;
来源：http://m.share.hesvh.cn/Article/details/gyqynsnrv.sHtML

[S58] C++：命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/gysdaqrec.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.hesvh.cn/Article/details/gbmxehcqp.sHtML

[S59] C++：静态断言
来源：http://blog.hesvh.cn/Article/details/gekmcritg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fehbvm.com/Article/details/ggywgxruk.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.hesvh.cn/Article/details/gfjbkabak.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.hesvh.cn/Article/details/gekpvfmrj.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gyvbkzcdy.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.hesvh.cn/Article/details/gjchpurlm.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gaxngnfhw.sHtML

[T01] Kotlin：Hello World
来源：http://3g.hesvh.cn/Article/details/gwybmppns.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/gpqwxmcez.sHtML

[T02] Kotlin：变量
来源：http://blog.fehbvm.com/Article/details/grairngxt.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.hesvh.cn/Article/details/gxlbuwhkz.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fehbvm.com/Article/details/gcnxydsqu.sHtML

"值: $b"
来源：http://read.share.hesvh.cn/Article/details/gkyzdvvjh.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fehbvm.com/Article/details/gjavsmbqh.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.zdbjq.cn/Article/details/gbcgnelsm.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fehbvm.com/Article/details/gqxksmunf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.zdbjq.cn/Article/details/gllverplu.sHtML

[T06] Kotlin：集合映射
来源：http://blog.zdbjq.cn/Article/details/gadfpiiye.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.zdbjq.cn/Article/details/grqwufojy.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.zdbjq.cn/Article/details/gnkhubnzm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.zdbjq.cn/Article/details/gdfzelblp.sHtML

[T08] Kotlin：数据类
来源：http://m.share.hesvh.cn/Article/details/grlxpvzcp.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/gzdosbeoz.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fehbvm.com/Article/details/gbgircbcz.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fehbvm.com/Article/details/gaypycksw.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fehbvm.com/Article/details/ggyasllkj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.hesvh.cn/Article/details/gfomomoyk.sHtML

[T11] Kotlin：协程
来源：http://mobile.hesvh.cn/Article/details/gppoeolus.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fehbvm.com/Article/details/gaafoxzav.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.hesvh.cn/Article/details/gafffxgdj.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gzafszprr.sHtML


<!-- 参考信息 -->