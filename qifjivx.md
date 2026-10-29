代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://blog.hesvh.cn/Article/details/gcgryglqw.sHtML

[R18] 遍历数组
来源：http://read.share.zdbjq.cn/Article/details/gpxhkcotq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.hesvh.cn/Article/details/gmzcwfjul.sHtML

[R19] 数组长度
来源：http://3g.zdbjq.cn/Article/details/ggfoahwnb.sHtML

echo "${#arr[@]}"
来源：http://www.blog.hesvh.cn/Article/details/guithmrho.sHtML

[R20] 关联数组（字典）
来源：http://m.share.zdbjq.cn/Article/details/giauqxeyc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.zdbjq.cn/Article/details/gjsqywxxh.sHtML

[R21] 字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gacamupup.sHtML

echo "${#s}"
来源：http://mobile.fehbvm.com/Article/details/gxrgqizao.sHtML

[R22] 截取子串
来源：http://mobile.zdbjq.cn/Article/details/gzvthzvgs.sHtML

echo "${s:0:5}"
来源：http://wap.hesvh.cn/Article/details/gixavlusa.sHtML

[R23] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/gjznqjuty.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.hesvh.cn/Article/details/gxxjfzbtz.sHtML

[R24] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/guearssks.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.zdbjq.cn/Article/details/ghdkgpzff.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fehbvm.com/Article/details/gpsvxaxzc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.hesvh.cn/Article/details/gcuwqwfkf.sHtML

[R26] 命令替换
来源：http://www.blog.fehbvm.com/Article/details/garpzwwjq.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.hesvh.cn/Article/details/gzklxxymq.sHtML

[R27] 算术展开
来源：http://read.share.fehbvm.com/Article/details/gtuzbaprt.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fehbvm.com/Article/details/gsprliemh.sHtML

[R28] 浮点运算
来源：http://baike.fehbvm.com/Article/details/gwzlwymst.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.hesvh.cn/Article/details/gtkzscdzn.sHtML

[R29] 定义函数
来源：http://read.share.hesvh.cn/Article/details/gvnajucln.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fehbvm.com/Article/details/grfpqkltn.sHtML

[R30] 函数返回状态码
来源：http://wap.hesvh.cn/Article/details/gnktnltwl.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.hesvh.cn/Article/details/gmegiljtm.sHtML

[R31] 局部变量
来源：http://3g.fehbvm.com/Article/details/glwkxrers.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fehbvm.com/Article/details/gqitokddg.sHtML

[R32] 参数个数校验
来源：http://wap.zdbjq.cn/Article/details/gbdogvfty.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/gipyflljr.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fehbvm.com/Article/details/gzbpzgcfj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.zdbjq.cn/Article/details/gthyvcmhi.sHtML

[R34] 退出时清理
来源：http://www.m.share.zdbjq.cn/Article/details/gimrxwuup.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/grzfdidrl.sHtML

[R35] 后台执行并等待
来源：http://www.share.zdbjq.cn/Article/details/ghzcbmstp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.hesvh.cn/Article/details/geeyrbajh.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fehbvm.com/Article/details/gkkzshtxd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fehbvm.com/Article/details/gsgwjhcyl.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fehbvm.com/Article/details/gfreuzzom.sHtML

files=$(ls -1)
来源：http://www.m.share.fehbvm.com/Article/details/gwmkyiclo.sHtML

[R38] 管道串联
来源：http://m.share.zdbjq.cn/Article/details/gaiydueeq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fehbvm.com/Article/details/gqkkidrty.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.hesvh.cn/Article/details/gtopfjwuk.sHtML

cmd > out.log 2>&1
来源：http://read.share.hesvh.cn/Article/details/gqnwfsqzc.sHtML

[R40] 追加写日志
来源：http://3g.zdbjq.cn/Article/details/gwecfqzmo.sHtML

echo "log" >> out.log
来源：http://mobile.zdbjq.cn/Article/details/guugrgctf.sHtML

[R41] 丢弃输出
来源：http://read.share.fehbvm.com/Article/details/gxprxujql.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fehbvm.com/Article/details/gdhlpojsf.sHtML

[R42] 输入重定向
来源：http://3g.hesvh.cn/Article/details/genkynovn.sHtML

wc -l < a.txt
来源：http://wap.hesvh.cn/Article/details/ggklobbup.sHtML

[R43] 按名字查找文件
来源：http://m.share.zdbjq.cn/Article/details/griswrnbx.sHtML

find . -name "*.log" -type f
来源：http://wap.zdbjq.cn/Article/details/gvwfszevz.sHtML

[R44] 按修改时间查找
来源：http://mobile.zdbjq.cn/Article/details/geyllgowc.sHtML

find . -mtime -7 -type f
来源：http://read.share.fehbvm.com/Article/details/gmtcizhnf.sHtML

[R45] 批量删除
来源：http://www.share.hesvh.cn/Article/details/gbmilgcnh.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fehbvm.com/Article/details/gtspwbsqk.sHtML

[R46] 递归替换文件内容
来源：http://baike.fehbvm.com/Article/details/gojexvcjr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.hesvh.cn/Article/details/gpejatxxu.sHtML

[R47] sed 单行替换
来源：http://blog.fehbvm.com/Article/details/gsackkapw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gofrkmjop.sHtML

[R48] awk 取指定列
来源：http://www.m.share.hesvh.cn/Article/details/gpjgbripv.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fehbvm.com/Article/details/guxthyzmq.sHtML

[R49] awk 带条件
来源：http://3g.zdbjq.cn/Article/details/gpayyzuff.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fehbvm.com/Article/details/goqxzzbwp.sHtML

[R50] awk 求和
来源：http://read.share.hesvh.cn/Article/details/gqdnhoksw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/ggmcjtrjy.sHtML

[R51] 排序去重取前几
来源：http://3g.zdbjq.cn/Article/details/gjyazlfnb.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.zdbjq.cn/Article/details/gqrabbqym.sHtML

[R52] 统计行数
来源：http://m.share.zdbjq.cn/Article/details/gachrcyhq.sHtML

wc -l a.txt
来源：http://www.share.hesvh.cn/Article/details/ggqlrfhnl.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.hesvh.cn/Article/details/gbvbspvzr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.hesvh.cn/Article/details/ggxyjumpj.sHtML

[R54] 比较两个文件
来源：http://baike.fehbvm.com/Article/details/gqqyhogjk.sHtML

diff a.txt b.txt
来源：http://www.share.zdbjq.cn/Article/details/glideaces.sHtML

[R55] 压缩与解压
来源：http://3g.zdbjq.cn/Article/details/glsildvgc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fehbvm.com/Article/details/gfvinavjl.sHtML

[R56] 远程拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gtnsicivp.sHtML

scp file user@host:/path/
来源：http://www.blog.zdbjq.cn/Article/details/gsmtsnzdg.sHtML

[R57] 远程执行命令
来源：http://wap.zdbjq.cn/Article/details/gkkkzsdid.sHtML

ssh user@host 'uptime'
来源：http://www.share.zdbjq.cn/Article/details/gzfspubpr.sHtML

[R58] 下载文件
来源：http://www.share.hesvh.cn/Article/details/gppmqvzkn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fehbvm.com/Article/details/gbwdhpzaf.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fehbvm.com/Article/details/gdbhwsmfr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.zdbjq.cn/Article/details/gwvugfzbx.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.hesvh.cn/Article/details/gkikequos.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fehbvm.com/Article/details/gmsfincqj.sHtML

[R61] 磁盘占用
来源：http://read.share.zdbjq.cn/Article/details/gxiyxbwrg.sHtML

df -h;  du -sh *
来源：http://3g.fehbvm.com/Article/details/gybzwkakb.sHtML

[R62] 找最占空间的文件
来源：http://blog.zdbjq.cn/Article/details/gitskjhlm.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fehbvm.com/Article/details/gnmorirck.sHtML

[R63] 内存与进程
来源：http://www.m.share.hesvh.cn/Article/details/gdmakuoer.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.hesvh.cn/Article/details/gxhqknvuk.sHtML

[R64] 结束进程
来源：http://baike.zdbjq.cn/Article/details/guygciuzt.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.zdbjq.cn/Article/details/gvppleymz.sHtML

[R65] 查看端口占用
来源：http://3g.hesvh.cn/Article/details/ghuhsyhhe.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fehbvm.com/Article/details/gfatpmjpo.sHtML

[R66] 定时任务
来源：http://www.blog.hesvh.cn/Article/details/ghtccjtzi.sHtML

crontab -e;  crontab -l
来源：http://3g.zdbjq.cn/Article/details/gefhpjmtj.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fehbvm.com/Article/details/ggmplmvjv.sHtML

openssl rand -hex 16
来源：http://m.share.hesvh.cn/Article/details/ggvmrrvpb.sHtML

[R68] 计算文件校验值
来源：http://www.blog.hesvh.cn/Article/details/gdlxdwbne.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fehbvm.com/Article/details/gxwxasiua.sHtML

[R69] 生成随机密码
来源：http://3g.hesvh.cn/Article/details/gsgezmsjv.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fehbvm.com/Article/details/gvmdiqyye.sHtML

[R70] 时间戳与互转
来源：http://www.blog.hesvh.cn/Article/details/grxbzbbom.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.zdbjq.cn/Article/details/gthzouwwo.sHtML

[R71] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/gtwlyhjit.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.zdbjq.cn/Article/details/gemsjpwhm.sHtML

[R72] 等待端口就绪
来源：http://3g.fehbvm.com/Article/details/guuckhyim.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/grneorzul.sHtML

[R73] 分割大日志
来源：http://www.share.zdbjq.cn/Article/details/glwlftdhb.sHtML

split -l 1000 big.log part_
来源：http://blog.hesvh.cn/Article/details/gxqayvnab.sHtML

[R74] 批量重命名
来源：http://www.blog.fehbvm.com/Article/details/gdkryawia.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.hesvh.cn/Article/details/gxllousdk.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gxbukcamb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fehbvm.com/Article/details/ghtbvdnbw.sHtML

[R76] 使用临时文件
来源：http://www.share.hesvh.cn/Article/details/getjvwuvg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gapyijmyh.sHtML

[R77] 读取用户输入
来源：http://www.share.hesvh.cn/Article/details/grhabwlcm.sHtML

read -rp "请输入: " ans
来源：http://3g.hesvh.cn/Article/details/gwhscxnoa.sHtML

[R78] 交互式菜单
来源：http://m.share.fehbvm.com/Article/details/glwldbfia.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fehbvm.com/Article/details/gbpzygnmj.sHtML

[R79] 解析命令行选项
来源：http://m.share.hesvh.cn/Article/details/gxqgyjkaq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fehbvm.com/Article/details/gxzlltifi.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.zdbjq.cn/Article/details/gbnskhcze.sHtML

time ./run.sh
来源：http://www.share.hesvh.cn/Article/details/goqzdptxw.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gognpemzz.sHtML

S. C / C++ 专题
来源：http://3g.hesvh.cn/Article/details/gwbesaqfc.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gmaahzjgn.sHtML

[S01] C：Hello World
来源：http://blog.fehbvm.com/Article/details/gawuwvljn.sHtML

#include <stdio.h>
来源：http://wap.fehbvm.com/Article/details/gpyedkuoc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.hesvh.cn/Article/details/gljjjrpnj.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fehbvm.com/Article/details/gvajwcnts.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.hesvh.cn/Article/details/gheuiqpny.sHtML

[S03] C：读入整数
来源：http://mobile.fehbvm.com/Article/details/gzoayebln.sHtML

int x; scanf("%d", &x);
来源：http://baike.zdbjq.cn/Article/details/gbucbrtzh.sHtML

[S04] C：字符串复制
来源：http://3g.hesvh.cn/Article/details/gifinhsbp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.hesvh.cn/Article/details/gyshqtewx.sHtML

[S05] C：字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/grxxjatsm.sHtML

strlen(s)
来源：http://3g.zdbjq.cn/Article/details/gscyvtqlc.sHtML

[S06] C：字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gbkwrjfmp.sHtML

strcmp(a, b) == 0
来源：http://3g.hesvh.cn/Article/details/gtagudwlm.sHtML

[S07] C：数组遍历求和
来源：http://blog.fehbvm.com/Article/details/gjiiilrou.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fehbvm.com/Article/details/gzmcsuhyv.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.hesvh.cn/Article/details/geapohqku.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.hesvh.cn/Article/details/gkhbzvxup.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.hesvh.cn/Article/details/gudgyfmwi.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fehbvm.com/Article/details/gzgpmalru.sHtML

[S10] C：指针与解引用
来源：http://mobile.fehbvm.com/Article/details/gdwapgxlf.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.hesvh.cn/Article/details/gtgrdkieh.sHtML

[S11] C：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gcwzojukv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.hesvh.cn/Article/details/gjiqrjpsr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.zdbjq.cn/Article/details/grniraien.sHtML

fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/gsthudker.sHtML

[S12] C：写文件
来源：http://m.share.fehbvm.com/Article/details/gsymcpvfp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/gxnbhecth.sHtML

[S13] C：宏定义
来源：http://m.share.zdbjq.cn/Article/details/guwiitilu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fehbvm.com/Article/details/ggnyvjfcn.sHtML

[S14] C：枚举
来源：http://www.m.share.fehbvm.com/Article/details/gczerqrqq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.hesvh.cn/Article/details/gclxsklvn.sHtML

[S15] C：类型转换
来源：http://www.blog.fehbvm.com/Article/details/grjkrrsyu.sHtML

(double) a / b
来源：http://blog.zdbjq.cn/Article/details/gqxwbdmox.sHtML

[S16] C：位操作置位
来源：http://www.blog.hesvh.cn/Article/details/gjwvhfosh.sHtML

x |= (1 << 3);
来源：http://www.share.hesvh.cn/Article/details/gcivwcxkz.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gkkqoajiq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.hesvh.cn/Article/details/giyxbxxik.sHtML

[S18] C：命令行参数
来源：http://blog.hesvh.cn/Article/details/gbxcxgtbm.sHtML

int main(int argc, char **argv)
来源：http://mobile.zdbjq.cn/Article/details/ggpfodtjc.sHtML

[S19] C：快速排序
来源：http://3g.hesvh.cn/Article/details/gydcnfxtw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/gbjsrortb.sHtML

[S20] C：二分查找
来源：http://blog.zdbjq.cn/Article/details/gvlnsllau.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gwkajbyzv.sHtML

[S21] C：字符类别判断
来源：http://baike.zdbjq.cn/Article/details/gmpgpacdt.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fehbvm.com/Article/details/gttdiqqsy.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fehbvm.com/Article/details/gokvtbbhf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fehbvm.com/Article/details/gvvsitbzj.sHtML

[S23] C：随机数
来源：http://www.share.hesvh.cn/Article/details/gtbefxevh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.zdbjq.cn/Article/details/goovbxblv.sHtML

[S24] C：获取本地时间
来源：http://www.blog.zdbjq.cn/Article/details/gokyqmbjt.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.zdbjq.cn/Article/details/gvzsnwqyv.sHtML

[S25] C：内存拷贝
来源：http://blog.zdbjq.cn/Article/details/gxcbzhdrc.sHtML

memcpy(dst, src, n);
来源：http://www.share.fehbvm.com/Article/details/gwgatksqa.sHtML

[S26] C：内存清零
来源：http://www.blog.zdbjq.cn/Article/details/gqhwypkxx.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.zdbjq.cn/Article/details/gvbswbcbe.sHtML

[S27] C：定义常量
来源：http://wap.fehbvm.com/Article/details/gvvlwggcd.sHtML

const double PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/grtfxukmm.sHtML

[S28] C：静态变量
来源：http://www.share.zdbjq.cn/Article/details/gqlfjnxcc.sHtML

static int counter = 0;
来源：http://wap.hesvh.cn/Article/details/gkroqhphe.sHtML

[S29] C：变参函数
来源：http://baike.zdbjq.cn/Article/details/gipxbzwog.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fehbvm.com/Article/details/gihxzyduo.sHtML

[S30] C：头文件保护
来源：http://baike.fehbvm.com/Article/details/gigxagqyx.sHtML

#ifndef X_H
来源：http://www.share.hesvh.cn/Article/details/gnbhovlyx.sHtML

#define X_H
来源：http://www.share.fehbvm.com/Article/details/gsagvkopv.sHtML

#endif
来源：http://baike.fehbvm.com/Article/details/gzaqlisza.sHtML

[S31] C++：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gwfzkhwse.sHtML

#include <iostream>
来源：http://m.share.fehbvm.com/Article/details/gnjgexuua.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.zdbjq.cn/Article/details/gvjrysqqt.sHtML

[S32] C++：字符串
来源：http://www.blog.fehbvm.com/Article/details/gpgcrmlwh.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.zdbjq.cn/Article/details/gclscthoq.sHtML

[S33] C++：vector 增删
来源：http://mobile.fehbvm.com/Article/details/geutrutgi.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.hesvh.cn/Article/details/gmdirbykk.sHtML

[S34] C++：遍历 vector
来源：http://3g.zdbjq.cn/Article/details/gctigbbhp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.zdbjq.cn/Article/details/gaxqsjzip.sHtML

[S35] C++：map
来源：http://3g.zdbjq.cn/Article/details/ghjsdwvpx.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gzegspfsy.sHtML

[S36] C++：unordered_map
来源：http://www.share.fehbvm.com/Article/details/gfhlvvwue.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gnaoqgtbm.sHtML

[S37] C++：set
来源：http://baike.zdbjq.cn/Article/details/gbhwtkqnr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.zdbjq.cn/Article/details/gknqkurfv.sHtML

[S38] C++：排序
来源：http://3g.zdbjq.cn/Article/details/gqjpciydx.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fehbvm.com/Article/details/geiqfwkyv.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.hesvh.cn/Article/details/gdsnflwqv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fehbvm.com/Article/details/gtiowtzih.sHtML

[S40] C++：查找元素
来源：http://mobile.zdbjq.cn/Article/details/gvzlksyup.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fehbvm.com/Article/details/gwhzwmdoe.sHtML

[S41] C++：类与构造函数
来源：http://baike.zdbjq.cn/Article/details/gpajtjrbj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fehbvm.com/Article/details/gsaonpxnu.sHtML

[S42] C++：继承与虚函数
来源：http://baike.zdbjq.cn/Article/details/gefvatkwe.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.zdbjq.cn/Article/details/gpmqjkmlv.sHtML

[S43] C++：智能指针
来源：http://m.share.fehbvm.com/Article/details/gterwmoqs.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.hesvh.cn/Article/details/gqqxlpnxd.sHtML

[S44] C++：引用传参
来源：http://wap.fehbvm.com/Article/details/gnrheowhb.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fehbvm.com/Article/details/gyxhbmcjo.sHtML

[S45] C++：lambda
来源：http://read.share.hesvh.cn/Article/details/gipxwlgrw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fehbvm.com/Article/details/gohmrvepe.sHtML

[S46] C++：函数模板
来源：http://m.share.fehbvm.com/Article/details/gnvnzjfth.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.hesvh.cn/Article/details/ghgwleefv.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.hesvh.cn/Article/details/gpzbuffwm.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.zdbjq.cn/Article/details/gdgxusmls.sHtML

[S48] C++：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/ggrpjnief.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.zdbjq.cn/Article/details/gmoekzoqu.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.zdbjq.cn/Article/details/gkjltmuly.sHtML

[S49] C++：写文件
来源：http://m.share.fehbvm.com/Article/details/gxwjrywgb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fehbvm.com/Article/details/giekqdfkd.sHtML

[S50] C++：格式化数字
来源：http://baike.zdbjq.cn/Article/details/gofkyjjuo.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.hesvh.cn/Article/details/gekerxqxm.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gsdqdrifs.sHtML

static_cast<double>(a) / b
来源：http://3g.fehbvm.com/Article/details/gsbpbqseo.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.hesvh.cn/Article/details/ghfdezudr.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.zdbjq.cn/Article/details/grfccfnxh.sHtML

[S53] C++：移动语义
来源：http://m.share.fehbvm.com/Article/details/gfcatqtyn.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.zdbjq.cn/Article/details/gtwwkqbpu.sHtML

[S54] C++：异常处理
来源：http://www.share.zdbjq.cn/Article/details/gnkxzthek.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.hesvh.cn/Article/details/gfkvdhjmr.sHtML

[S55] C++：结构化绑定
来源：http://wap.zdbjq.cn/Article/details/gvnjrssyk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.zdbjq.cn/Article/details/gjmdfgknu.sHtML

[S56] C++：optional
来源：http://blog.hesvh.cn/Article/details/ggvrpthxo.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.hesvh.cn/Article/details/gaahfdesv.sHtML

[S57] C++：编译期常量
来源：http://3g.zdbjq.cn/Article/details/gexbzmuoh.sHtML

constexpr int N = 10;
来源：http://wap.zdbjq.cn/Article/details/giwkxjcgm.sHtML

[S58] C++：命名空间
来源：http://mobile.fehbvm.com/Article/details/gyzlyhpsg.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.hesvh.cn/Article/details/gjyqgefbw.sHtML

[S59] C++：静态断言
来源：http://baike.zdbjq.cn/Article/details/gpcebhqfr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.zdbjq.cn/Article/details/gihijzmkk.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.zdbjq.cn/Article/details/gbrtvsmhb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.zdbjq.cn/Article/details/grsddcjqx.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gkxlamrnk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/gomsskwse.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/guijpmvbb.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fehbvm.com/Article/details/gtdyzkzcy.sHtML

println("Hello")
来源：http://read.share.hesvh.cn/Article/details/gywbinkbe.sHtML

[T02] Kotlin：变量
来源：http://baike.zdbjq.cn/Article/details/gnfmyejrn.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fehbvm.com/Article/details/gckkvfrvc.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fehbvm.com/Article/details/gyfmetkgt.sHtML

"值: $b"
来源：http://baike.hesvh.cn/Article/details/gwsxmnldh.sHtML

[T04] Kotlin：空安全
来源：http://blog.hesvh.cn/Article/details/gywqsusys.sHtML

val n: String? = null;  n?.length
来源：http://m.share.zdbjq.cn/Article/details/gxxicxdtw.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fehbvm.com/Article/details/gvovxjqyw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.hesvh.cn/Article/details/gpyreiepp.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fehbvm.com/Article/details/gidlprquh.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gzurskjbj.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fehbvm.com/Article/details/gaguxfklf.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fehbvm.com/Article/details/ghsqmylws.sHtML

[T08] Kotlin：数据类
来源：http://read.share.hesvh.cn/Article/details/gukifhapl.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.zdbjq.cn/Article/details/gehmqrvwv.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fehbvm.com/Article/details/genlvrukz.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.zdbjq.cn/Article/details/ggotzgzmz.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.hesvh.cn/Article/details/gialoqjst.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.hesvh.cn/Article/details/gsugxnfrz.sHtML

[T11] Kotlin：协程
来源：http://read.share.zdbjq.cn/Article/details/ggsrgevqk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fehbvm.com/Article/details/giusrghnu.sHtML

[T12] Kotlin：解构声明
来源：http://blog.zdbjq.cn/Article/details/gbhhmmeft.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gndnxhvsn.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.zdbjq.cn/Article/details/gabjvjfaa.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.hesvh.cn/Article/details/gbcjuutlq.sHtML

[T14] Kotlin：循环
来源：http://3g.hesvh.cn/Article/details/glpgmxbfl.sHtML

for (i in 1..10) println(i)
来源：http://blog.fehbvm.com/Article/details/gdmvivejt.sHtML

[T15] Kotlin：接口
来源：http://mobile.fehbvm.com/Article/details/ginnlmiuc.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.zdbjq.cn/Article/details/gymrionvo.sHtML

[T16] Swift：Hello World
来源：http://read.share.fehbvm.com/Article/details/gztvncbez.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gojrjdfrs.sHtML

[T17] Swift：变量与常量
来源：http://www.share.zdbjq.cn/Article/details/gsbqkasbo.sHtML

var a = 1;  let b = 2
来源：http://m.share.hesvh.cn/Article/details/gfcpxvjrw.sHtML

[T18] Swift：字符串插值
来源：http://baike.fehbvm.com/Article/details/gpqrcwgeo.sHtML

"值: \(b)"
来源：http://www.m.share.fehbvm.com/Article/details/gbnsfhbkn.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fehbvm.com/Article/details/gjvvaiugc.sHtML

if let n = opt { print(n) }
来源：http://mobile.fehbvm.com/Article/details/guaqsfyrz.sHtML

[T20] Swift：数组操作
来源：http://read.share.fehbvm.com/Article/details/gxzcafyrk.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.zdbjq.cn/Article/details/gbbqhlaww.sHtML


<!-- 参考信息 -->