代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fehbvm.com/Article/details/gssslhscs.sHtML

[R10] 正则匹配
来源：http://read.share.zdbjq.cn/Article/details/ghcdbohot.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.hesvh.cn/Article/details/guvaibmzi.sHtML

[R11] case 多分支
来源：http://m.share.zdbjq.cn/Article/details/gluicsmcl.sHtML

case "$1" in
来源：http://www.share.fehbvm.com/Article/details/ghrjwoybh.sHtML

start) echo "启动" ;;
来源：http://mobile.zdbjq.cn/Article/details/gytntsxpm.sHtML

stop)  echo "停止" ;;
来源：http://m.share.zdbjq.cn/Article/details/guttpuktw.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fehbvm.com/Article/details/glpammncw.sHtML

esac
来源：http://www.blog.fehbvm.com/Article/details/goafonadg.sHtML

[R12] for 遍历文件
来源：http://mobile.hesvh.cn/Article/details/gqehxnhes.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fehbvm.com/Article/details/gznykwvdh.sHtML

[R13] for 计数循环
来源：http://m.share.zdbjq.cn/Article/details/glyopumds.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gmgjmxpbf.sHtML

[R14] C 风格 for
来源：http://wap.fehbvm.com/Article/details/gmsfujfad.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/gxvadqjje.sHtML

[R15] while 逐行读文件
来源：http://3g.fehbvm.com/Article/details/gagjaifpj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fehbvm.com/Article/details/gmenxmekd.sHtML

[R16] until 等待条件
来源：http://mobile.hesvh.cn/Article/details/gaglqdxgc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gqjkpmshm.sHtML

[R17] 数组定义与取值
来源：http://blog.hesvh.cn/Article/details/gdjtjblwr.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.zdbjq.cn/Article/details/glqvhxqry.sHtML

[R18] 遍历数组
来源：http://m.share.hesvh.cn/Article/details/gjcarecpo.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.zdbjq.cn/Article/details/gouxbemru.sHtML

[R19] 数组长度
来源：http://www.share.fehbvm.com/Article/details/gzlzxcdss.sHtML

echo "${#arr[@]}"
来源：http://read.share.fehbvm.com/Article/details/gsjuasqnf.sHtML

[R20] 关联数组（字典）
来源：http://blog.fehbvm.com/Article/details/gdeaegivz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.hesvh.cn/Article/details/gpqtxyeix.sHtML

[R21] 字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gfgumntco.sHtML

echo "${#s}"
来源：http://m.share.fehbvm.com/Article/details/gvwscgeps.sHtML

[R22] 截取子串
来源：http://3g.zdbjq.cn/Article/details/gqylbhoyd.sHtML

echo "${s:0:5}"
来源：http://baike.hesvh.cn/Article/details/grakyhknb.sHtML

[R23] 字符串替换
来源：http://blog.fehbvm.com/Article/details/gfpmdbeem.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fehbvm.com/Article/details/geyugfnwd.sHtML

[R24] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gxrpcvmig.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.hesvh.cn/Article/details/gynzooxzg.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.zdbjq.cn/Article/details/gevnktbyp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.zdbjq.cn/Article/details/gtfsaoqzh.sHtML

[R26] 命令替换
来源：http://www.blog.zdbjq.cn/Article/details/gcamcqqyz.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fehbvm.com/Article/details/gvetnpklv.sHtML

[R27] 算术展开
来源：http://blog.hesvh.cn/Article/details/gfpsxrmuc.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.hesvh.cn/Article/details/gihhawhcc.sHtML

[R28] 浮点运算
来源：http://baike.zdbjq.cn/Article/details/gjdvsvjiy.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.zdbjq.cn/Article/details/ghynsxdjy.sHtML

[R29] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/gobtjnhke.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.zdbjq.cn/Article/details/ghzckxfnm.sHtML

[R30] 函数返回状态码
来源：http://mobile.hesvh.cn/Article/details/gyjmgisoj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fehbvm.com/Article/details/gewmaakkm.sHtML

[R31] 局部变量
来源：http://www.share.hesvh.cn/Article/details/gzcxurpdh.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.zdbjq.cn/Article/details/grnaoylbe.sHtML

[R32] 参数个数校验
来源：http://3g.hesvh.cn/Article/details/gbhxjntav.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/gqhsnpqwo.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.hesvh.cn/Article/details/gcffywagm.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.zdbjq.cn/Article/details/gmbbhkygm.sHtML

[R34] 退出时清理
来源：http://wap.hesvh.cn/Article/details/gnbuxthqk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.zdbjq.cn/Article/details/gtkfgiixo.sHtML

[R35] 后台执行并等待
来源：http://mobile.hesvh.cn/Article/details/guamrbkov.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.hesvh.cn/Article/details/gzidignum.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.hesvh.cn/Article/details/glncugjgp.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.zdbjq.cn/Article/details/gtlvyhmyi.sHtML

[R37] 把输出赋给变量
来源：http://3g.hesvh.cn/Article/details/gggerapsr.sHtML

files=$(ls -1)
来源：http://blog.hesvh.cn/Article/details/gmflptczf.sHtML

[R38] 管道串联
来源：http://www.blog.fehbvm.com/Article/details/giwmdxhpp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.hesvh.cn/Article/details/glprtvpkt.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.hesvh.cn/Article/details/gjrbsshwn.sHtML

cmd > out.log 2>&1
来源：http://wap.zdbjq.cn/Article/details/goataailq.sHtML

[R40] 追加写日志
来源：http://3g.fehbvm.com/Article/details/gzgpachpo.sHtML

echo "log" >> out.log
来源：http://read.share.fehbvm.com/Article/details/gxaorvdgv.sHtML

[R41] 丢弃输出
来源：http://read.share.hesvh.cn/Article/details/ggyhypbus.sHtML

cmd >/dev/null 2>&1
来源：http://wap.hesvh.cn/Article/details/gjetvhvyw.sHtML

[R42] 输入重定向
来源：http://www.m.share.fehbvm.com/Article/details/goilqmiwz.sHtML

wc -l < a.txt
来源：http://3g.zdbjq.cn/Article/details/gtjnixgqu.sHtML

[R43] 按名字查找文件
来源：http://www.blog.zdbjq.cn/Article/details/gqmjurvua.sHtML

find . -name "*.log" -type f
来源：http://www.blog.zdbjq.cn/Article/details/ggzvkhmta.sHtML

[R44] 按修改时间查找
来源：http://blog.fehbvm.com/Article/details/gimjhrwgp.sHtML

find . -mtime -7 -type f
来源：http://3g.zdbjq.cn/Article/details/gnxbnxsbv.sHtML

[R45] 批量删除
来源：http://wap.fehbvm.com/Article/details/gifllcdyb.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.zdbjq.cn/Article/details/gxpwhoqod.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fehbvm.com/Article/details/ghmhoiftn.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.zdbjq.cn/Article/details/gzpemvvhj.sHtML

[R47] sed 单行替换
来源：http://3g.zdbjq.cn/Article/details/gekdlubir.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fehbvm.com/Article/details/gsgqsqbre.sHtML

[R48] awk 取指定列
来源：http://3g.hesvh.cn/Article/details/gfcfoofaf.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gvaexzhfr.sHtML

[R49] awk 带条件
来源：http://baike.fehbvm.com/Article/details/gvlefwibn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fehbvm.com/Article/details/gzxelkwax.sHtML

[R50] awk 求和
来源：http://www.share.hesvh.cn/Article/details/gnuyycvxw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gkxikliya.sHtML

[R51] 排序去重取前几
来源：http://wap.hesvh.cn/Article/details/getbwbwef.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.hesvh.cn/Article/details/gkbcgsirh.sHtML

[R52] 统计行数
来源：http://www.blog.zdbjq.cn/Article/details/ggzccdbvm.sHtML

wc -l a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/growlysyb.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fehbvm.com/Article/details/gdbkgoepz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.zdbjq.cn/Article/details/gqadfavug.sHtML

[R54] 比较两个文件
来源：http://wap.zdbjq.cn/Article/details/gdkvqghzv.sHtML

diff a.txt b.txt
来源：http://wap.fehbvm.com/Article/details/gejjpvvvk.sHtML

[R55] 压缩与解压
来源：http://m.share.zdbjq.cn/Article/details/guvmpdejm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.hesvh.cn/Article/details/gbokdbxfi.sHtML

[R56] 远程拷贝
来源：http://www.blog.fehbvm.com/Article/details/gstpthmgx.sHtML

scp file user@host:/path/
来源：http://wap.fehbvm.com/Article/details/ginhtortc.sHtML

[R57] 远程执行命令
来源：http://www.share.hesvh.cn/Article/details/gsrrwuwhz.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.zdbjq.cn/Article/details/gfdplkwle.sHtML

[R58] 下载文件
来源：http://www.m.share.zdbjq.cn/Article/details/gsnloioeq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.hesvh.cn/Article/details/gfrhlimwq.sHtML

[R59] 发 POST JSON
来源：http://blog.hesvh.cn/Article/details/gagwdmhbq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fehbvm.com/Article/details/gjzobuuis.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/gxzkhoskp.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.hesvh.cn/Article/details/gvwqrnpva.sHtML

[R61] 磁盘占用
来源：http://3g.fehbvm.com/Article/details/gtnrzwtbd.sHtML

df -h;  du -sh *
来源：http://www.share.fehbvm.com/Article/details/gqtbbeyvi.sHtML

[R62] 找最占空间的文件
来源：http://wap.fehbvm.com/Article/details/ghzorslah.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.zdbjq.cn/Article/details/gatulldiv.sHtML

[R63] 内存与进程
来源：http://www.blog.zdbjq.cn/Article/details/gjiyhmekh.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.hesvh.cn/Article/details/gcpoyuqzx.sHtML

[R64] 结束进程
来源：http://read.share.hesvh.cn/Article/details/ggmqwcrol.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fehbvm.com/Article/details/gnbnzjxoh.sHtML

[R65] 查看端口占用
来源：http://m.share.hesvh.cn/Article/details/gwwuecupf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fehbvm.com/Article/details/gjlzaxavg.sHtML

[R66] 定时任务
来源：http://www.m.share.fehbvm.com/Article/details/giagpqsfd.sHtML

crontab -e;  crontab -l
来源：http://read.share.hesvh.cn/Article/details/gvwlugjrr.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fehbvm.com/Article/details/gurmgabpw.sHtML

openssl rand -hex 16
来源：http://www.share.zdbjq.cn/Article/details/gbmlkaldc.sHtML

[R68] 计算文件校验值
来源：http://3g.fehbvm.com/Article/details/guvwkfalk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.hesvh.cn/Article/details/giirbvxjp.sHtML

[R69] 生成随机密码
来源：http://baike.fehbvm.com/Article/details/giekqadzj.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.hesvh.cn/Article/details/gocsjerdr.sHtML

[R70] 时间戳与互转
来源：http://baike.hesvh.cn/Article/details/gogqxrevv.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fehbvm.com/Article/details/grsajrlpm.sHtML

[R71] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gfdpjogdz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.hesvh.cn/Article/details/gmlbtuznl.sHtML

[R72] 等待端口就绪
来源：http://wap.hesvh.cn/Article/details/ggdnenruj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/gsallucgq.sHtML

[R73] 分割大日志
来源：http://baike.zdbjq.cn/Article/details/gvccfqjzy.sHtML

split -l 1000 big.log part_
来源：http://baike.hesvh.cn/Article/details/gflftgwby.sHtML

[R74] 批量重命名
来源：http://www.share.hesvh.cn/Article/details/grrfxehpn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.hesvh.cn/Article/details/goyvuaonr.sHtML

[R75] 导出环境变量
来源：http://wap.hesvh.cn/Article/details/gcymqdtwy.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fehbvm.com/Article/details/gprrdkzal.sHtML

[R76] 使用临时文件
来源：http://blog.zdbjq.cn/Article/details/gaikdldav.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/gmjctzijj.sHtML

[R77] 读取用户输入
来源：http://blog.hesvh.cn/Article/details/gangwhzct.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.hesvh.cn/Article/details/gztsvydxi.sHtML

[R78] 交互式菜单
来源：http://www.blog.fehbvm.com/Article/details/gcnsbrslq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.hesvh.cn/Article/details/gukdiwngw.sHtML

[R79] 解析命令行选项
来源：http://read.share.hesvh.cn/Article/details/gbneywkaa.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.hesvh.cn/Article/details/gbqvrdycq.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.zdbjq.cn/Article/details/gpbzsqziy.sHtML

time ./run.sh
来源：http://blog.hesvh.cn/Article/details/gbaxprrot.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/geliqubpy.sHtML

S. C / C++ 专题
来源：http://blog.zdbjq.cn/Article/details/gfnroaeah.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gpjeswsmu.sHtML

[S01] C：Hello World
来源：http://blog.hesvh.cn/Article/details/gauslttsc.sHtML

#include <stdio.h>
来源：http://blog.fehbvm.com/Article/details/gibxowakg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fehbvm.com/Article/details/gvfxdhnmy.sHtML

[S02] C：变量与格式化输出
来源：http://3g.hesvh.cn/Article/details/gkdkhujuk.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.zdbjq.cn/Article/details/gadtuhapg.sHtML

[S03] C：读入整数
来源：http://m.share.zdbjq.cn/Article/details/grwdytjwq.sHtML

int x; scanf("%d", &x);
来源：http://www.share.zdbjq.cn/Article/details/goevydnap.sHtML

[S04] C：字符串复制
来源：http://m.share.fehbvm.com/Article/details/gnfddjoax.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gjseshopv.sHtML

[S05] C：字符串长度
来源：http://wap.fehbvm.com/Article/details/gtiyvokwo.sHtML

strlen(s)
来源：http://3g.zdbjq.cn/Article/details/ghgottotj.sHtML

[S06] C：字符串比较
来源：http://3g.fehbvm.com/Article/details/gvehkutfh.sHtML

strcmp(a, b) == 0
来源：http://m.share.zdbjq.cn/Article/details/gfdwmrwmu.sHtML

[S07] C：数组遍历求和
来源：http://baike.hesvh.cn/Article/details/gcadnfcjm.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.hesvh.cn/Article/details/gvzpcvlcj.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.hesvh.cn/Article/details/guoelgrzj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.hesvh.cn/Article/details/gnwctufgk.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.hesvh.cn/Article/details/gvwygtfwj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.hesvh.cn/Article/details/gdpsrhwlk.sHtML

[S10] C：指针与解引用
来源：http://3g.fehbvm.com/Article/details/gldcnramy.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fehbvm.com/Article/details/galemounu.sHtML

[S11] C：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/ghhwleztp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fehbvm.com/Article/details/gwngwuxao.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.zdbjq.cn/Article/details/gmstjszln.sHtML

fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gzcvhlyhb.sHtML

[S12] C：写文件
来源：http://3g.hesvh.cn/Article/details/ggnngfpqp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fehbvm.com/Article/details/gbnmlujny.sHtML

[S13] C：宏定义
来源：http://m.share.hesvh.cn/Article/details/gakwylmeu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.zdbjq.cn/Article/details/gaahqruai.sHtML

[S14] C：枚举
来源：http://3g.hesvh.cn/Article/details/gqwdmddrg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fehbvm.com/Article/details/gqenevlpo.sHtML

[S15] C：类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gwtydmmhi.sHtML

(double) a / b
来源：http://wap.hesvh.cn/Article/details/gmnipooet.sHtML

[S16] C：位操作置位
来源：http://m.share.zdbjq.cn/Article/details/gszvvyqbn.sHtML

x |= (1 << 3);
来源：http://baike.hesvh.cn/Article/details/gflxsizdp.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gidyfccwk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.hesvh.cn/Article/details/grynhbcos.sHtML

[S18] C：命令行参数
来源：http://baike.fehbvm.com/Article/details/gsthrdrqv.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.hesvh.cn/Article/details/gimhsvehu.sHtML

[S19] C：快速排序
来源：http://www.m.share.zdbjq.cn/Article/details/gppydxrri.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/glylpfevx.sHtML

[S20] C：二分查找
来源：http://www.share.hesvh.cn/Article/details/gzoqeisng.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gnidgqfly.sHtML

[S21] C：字符类别判断
来源：http://mobile.hesvh.cn/Article/details/gharxdgcx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.hesvh.cn/Article/details/gllandzub.sHtML

[S22] C：字符串转数字
来源：http://3g.hesvh.cn/Article/details/gyevejemw.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.hesvh.cn/Article/details/gkykoquoy.sHtML

[S23] C：随机数
来源：http://m.share.hesvh.cn/Article/details/ggplfjpap.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.zdbjq.cn/Article/details/gkoqfyotd.sHtML

[S24] C：获取本地时间
来源：http://www.share.fehbvm.com/Article/details/gbdprhooh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.zdbjq.cn/Article/details/gpzmrtlyb.sHtML

[S25] C：内存拷贝
来源：http://blog.hesvh.cn/Article/details/gctowiobn.sHtML

memcpy(dst, src, n);
来源：http://wap.zdbjq.cn/Article/details/gzltmbijt.sHtML

[S26] C：内存清零
来源：http://3g.fehbvm.com/Article/details/glqqyabjv.sHtML

memset(a, 0, sizeof a);
来源：http://3g.zdbjq.cn/Article/details/gheqogscy.sHtML

[S27] C：定义常量
来源：http://mobile.zdbjq.cn/Article/details/gcrjafinq.sHtML

const double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gzlhxkojc.sHtML

[S28] C：静态变量
来源：http://www.share.fehbvm.com/Article/details/gbzhtthga.sHtML

static int counter = 0;
来源：http://m.share.zdbjq.cn/Article/details/gbbenmxnq.sHtML

[S29] C：变参函数
来源：http://read.share.hesvh.cn/Article/details/gooxzjwjn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.zdbjq.cn/Article/details/gwtaqhrru.sHtML

[S30] C：头文件保护
来源：http://read.share.fehbvm.com/Article/details/gtexiehbw.sHtML

#ifndef X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gwjmyncly.sHtML

#define X_H
来源：http://mobile.fehbvm.com/Article/details/golfyfvns.sHtML

#endif
来源：http://baike.hesvh.cn/Article/details/gedieoxfo.sHtML

[S31] C++：Hello World
来源：http://read.share.hesvh.cn/Article/details/goyfdivgx.sHtML

#include <iostream>
来源：http://www.blog.hesvh.cn/Article/details/gqxbgztpu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.zdbjq.cn/Article/details/gbwpetcxl.sHtML

[S32] C++：字符串
来源：http://wap.fehbvm.com/Article/details/gxntmqiwo.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.hesvh.cn/Article/details/ghdkhqdpt.sHtML

[S33] C++：vector 增删
来源：http://3g.fehbvm.com/Article/details/ghdnncvah.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.zdbjq.cn/Article/details/gasnhhfjy.sHtML

[S34] C++：遍历 vector
来源：http://www.share.hesvh.cn/Article/details/gtcheonqo.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.zdbjq.cn/Article/details/gnrqkxxdf.sHtML

[S35] C++：map
来源：http://baike.fehbvm.com/Article/details/giwuzbhnb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gizhpzaig.sHtML

[S36] C++：unordered_map
来源：http://mobile.fehbvm.com/Article/details/gifxysvqh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/ggvqlaiai.sHtML

[S37] C++：set
来源：http://read.share.hesvh.cn/Article/details/gsxctdmwy.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fehbvm.com/Article/details/gsuabtdej.sHtML

[S38] C++：排序
来源：http://www.share.fehbvm.com/Article/details/gdiqkesdl.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fehbvm.com/Article/details/gdrfvmehu.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fehbvm.com/Article/details/gegmnstht.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.hesvh.cn/Article/details/gterjitfy.sHtML

[S40] C++：查找元素
来源：http://blog.zdbjq.cn/Article/details/gktnmudil.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.zdbjq.cn/Article/details/glwsenfbg.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.zdbjq.cn/Article/details/giciltsoq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.zdbjq.cn/Article/details/gwqkmbmlw.sHtML

[S42] C++：继承与虚函数
来源：http://baike.zdbjq.cn/Article/details/gqvjvaluq.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.zdbjq.cn/Article/details/gwjhlhhhp.sHtML

[S43] C++：智能指针
来源：http://m.share.zdbjq.cn/Article/details/gjinncnoy.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.zdbjq.cn/Article/details/gcxztjtpm.sHtML

[S44] C++：引用传参
来源：http://read.share.zdbjq.cn/Article/details/gydvwntjr.sHtML

void inc(int &x) { ++x; }
来源：http://wap.hesvh.cn/Article/details/gstlwmcvm.sHtML

[S45] C++：lambda
来源：http://baike.fehbvm.com/Article/details/gipaxgjvg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.hesvh.cn/Article/details/gbsrpexbd.sHtML

[S46] C++：函数模板
来源：http://mobile.zdbjq.cn/Article/details/gxudtickg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.hesvh.cn/Article/details/gvfabzbka.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fehbvm.com/Article/details/gtjlzvnof.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fehbvm.com/Article/details/gwtxruyoo.sHtML

[S48] C++：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gqlvulwjv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.hesvh.cn/Article/details/gephmunml.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fehbvm.com/Article/details/gumuwhvny.sHtML

[S49] C++：写文件
来源：http://baike.hesvh.cn/Article/details/gxrfzmuzc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.zdbjq.cn/Article/details/gipkpgcdh.sHtML

[S50] C++：格式化数字
来源：http://www.share.zdbjq.cn/Article/details/gvqrmqvkg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gqzmzjbot.sHtML

[S51] C++：显式类型转换
来源：http://mobile.zdbjq.cn/Article/details/glkjzsllz.sHtML

static_cast<double>(a) / b
来源：http://3g.hesvh.cn/Article/details/gwlhbkrjo.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.hesvh.cn/Article/details/gibvbthtf.sHtML

int size() const noexcept { return n_; }
来源：http://baike.hesvh.cn/Article/details/gcztbdmok.sHtML

[S53] C++：移动语义
来源：http://www.m.share.hesvh.cn/Article/details/gqsfuueee.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fehbvm.com/Article/details/gljyyndbr.sHtML

[S54] C++：异常处理
来源：http://3g.hesvh.cn/Article/details/gmiiaivnv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.hesvh.cn/Article/details/ghowvfdht.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.zdbjq.cn/Article/details/gqrzaifdo.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.hesvh.cn/Article/details/gnphtmbup.sHtML

[S56] C++：optional
来源：http://m.share.fehbvm.com/Article/details/grjieuzdo.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fehbvm.com/Article/details/gnrcnlfgv.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.hesvh.cn/Article/details/gqzbwrrll.sHtML

constexpr int N = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gcqciwdsl.sHtML

[S58] C++：命名空间
来源：http://read.share.hesvh.cn/Article/details/gnxerktjd.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.hesvh.cn/Article/details/gjxlbabps.sHtML

[S59] C++：静态断言
来源：http://read.share.zdbjq.cn/Article/details/gbeuzsgcl.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.hesvh.cn/Article/details/gldizmdzv.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.zdbjq.cn/Article/details/galirfghf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fehbvm.com/Article/details/gytafgzfr.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/garxonuxf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fehbvm.com/Article/details/gxogyrbdt.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gikzzieku.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fehbvm.com/Article/details/gftxgcbtn.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gqviukfcl.sHtML

[T02] Kotlin：变量
来源：http://baike.fehbvm.com/Article/details/gygimhoex.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.zdbjq.cn/Article/details/giaxemkai.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.zdbjq.cn/Article/details/gnmdsopha.sHtML

"值: $b"
来源：http://blog.zdbjq.cn/Article/details/gkiyhgkiz.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.hesvh.cn/Article/details/gxqhepwfj.sHtML

val n: String? = null;  n?.length
来源：http://www.share.hesvh.cn/Article/details/ggwphkisj.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.zdbjq.cn/Article/details/gjpxgwlna.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.zdbjq.cn/Article/details/gxfhpboae.sHtML

[T06] Kotlin：集合映射
来源：http://baike.zdbjq.cn/Article/details/gqvnoegqv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gfcyeosvy.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.zdbjq.cn/Article/details/glrwjelae.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fehbvm.com/Article/details/gewtndxqd.sHtML

[T08] Kotlin：数据类
来源：http://wap.hesvh.cn/Article/details/gcfyuvcey.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.hesvh.cn/Article/details/gnubucthq.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.hesvh.cn/Article/details/gsmeqzzna.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.zdbjq.cn/Article/details/gfzxswtin.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.hesvh.cn/Article/details/gkvvdglof.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.hesvh.cn/Article/details/gomgzxiyo.sHtML


<!-- 参考信息 -->