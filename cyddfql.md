代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.zdbjq.cn/Article/details/ggizqmqru.sHtML

[R10] 正则匹配
来源：http://www.blog.zdbjq.cn/Article/details/gurfzuybj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fehbvm.com/Article/details/gtbhsewpj.sHtML

[R11] case 多分支
来源：http://www.share.hesvh.cn/Article/details/gnfujjvfu.sHtML

case "$1" in
来源：http://www.blog.fehbvm.com/Article/details/gaoiicaql.sHtML

start) echo "启动" ;;
来源：http://3g.fehbvm.com/Article/details/gmqexewxk.sHtML

stop)  echo "停止" ;;
来源：http://wap.hesvh.cn/Article/details/gvjjovqtj.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gwwioddau.sHtML

esac
来源：http://baike.zdbjq.cn/Article/details/gmhrgsxmq.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fehbvm.com/Article/details/gppnylrou.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.zdbjq.cn/Article/details/gdzaatjcg.sHtML

[R13] for 计数循环
来源：http://wap.zdbjq.cn/Article/details/goievvvra.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/gpnieqfqy.sHtML

[R14] C 风格 for
来源：http://blog.fehbvm.com/Article/details/gehvszqpa.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/gulczbqax.sHtML

[R15] while 逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gmdvczjqs.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.zdbjq.cn/Article/details/gjoakvthd.sHtML

[R16] until 等待条件
来源：http://www.m.share.zdbjq.cn/Article/details/gpxkqwtrv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/gvxkplptc.sHtML

[R17] 数组定义与取值
来源：http://blog.fehbvm.com/Article/details/gksiwnywl.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.hesvh.cn/Article/details/gewtkmcbl.sHtML

[R18] 遍历数组
来源：http://baike.fehbvm.com/Article/details/gvopgylmf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fehbvm.com/Article/details/gfpspqrck.sHtML

[R19] 数组长度
来源：http://www.blog.hesvh.cn/Article/details/gnhtxvlmt.sHtML

echo "${#arr[@]}"
来源：http://www.blog.hesvh.cn/Article/details/gcpjkqieq.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fehbvm.com/Article/details/gaqbjiqdo.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.hesvh.cn/Article/details/glvxhwkfz.sHtML

[R21] 字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gxqmiapfd.sHtML

echo "${#s}"
来源：http://blog.hesvh.cn/Article/details/gxajtsnns.sHtML

[R22] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/gtysvdltc.sHtML

echo "${s:0:5}"
来源：http://mobile.hesvh.cn/Article/details/gugoxwfuz.sHtML

[R23] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/gaeqorzzn.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.hesvh.cn/Article/details/gotteowne.sHtML

[R24] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/gdnqsqsga.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fehbvm.com/Article/details/gdcnpeeyt.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.zdbjq.cn/Article/details/ggwhrxogk.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fehbvm.com/Article/details/gdwqffrrq.sHtML

[R26] 命令替换
来源：http://blog.hesvh.cn/Article/details/gxjrzfeug.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.zdbjq.cn/Article/details/gprysdwpa.sHtML

[R27] 算术展开
来源：http://m.share.zdbjq.cn/Article/details/ghcclxnrc.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fehbvm.com/Article/details/gkkftlafu.sHtML

[R28] 浮点运算
来源：http://www.m.share.hesvh.cn/Article/details/gbauvrwel.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.hesvh.cn/Article/details/ghsyujhbz.sHtML

[R29] 定义函数
来源：http://blog.hesvh.cn/Article/details/grykjumcs.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fehbvm.com/Article/details/gqagkftdx.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gvcyejpnn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fehbvm.com/Article/details/gfkwvikjj.sHtML

[R31] 局部变量
来源：http://mobile.hesvh.cn/Article/details/gqgjldziu.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.hesvh.cn/Article/details/gxmbmmwjq.sHtML

[R32] 参数个数校验
来源：http://read.share.hesvh.cn/Article/details/gueirumlp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/gmklpmzkl.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fehbvm.com/Article/details/goqfrxdmq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.zdbjq.cn/Article/details/gcvzgwngd.sHtML

[R34] 退出时清理
来源：http://read.share.hesvh.cn/Article/details/ghuydnmjq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/gfanhurel.sHtML

[R35] 后台执行并等待
来源：http://mobile.hesvh.cn/Article/details/gfzddhxqa.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fehbvm.com/Article/details/gfwgfnlpb.sHtML

[R36] 并发执行多个任务
来源：http://baike.fehbvm.com/Article/details/ggtwvlzmt.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.hesvh.cn/Article/details/gponvdenh.sHtML

[R37] 把输出赋给变量
来源：http://wap.fehbvm.com/Article/details/gplwlwbno.sHtML

files=$(ls -1)
来源：http://baike.fehbvm.com/Article/details/gaepezqyt.sHtML

[R38] 管道串联
来源：http://3g.hesvh.cn/Article/details/gnbkwqxgw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.zdbjq.cn/Article/details/grdcbsmdf.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.zdbjq.cn/Article/details/grugwbhjd.sHtML

cmd > out.log 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gbbmelotm.sHtML

[R40] 追加写日志
来源：http://baike.fehbvm.com/Article/details/ghmmohxvo.sHtML

echo "log" >> out.log
来源：http://baike.hesvh.cn/Article/details/gqypfqnoe.sHtML

[R41] 丢弃输出
来源：http://read.share.fehbvm.com/Article/details/glcagoces.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/giavmfyqo.sHtML

[R42] 输入重定向
来源：http://m.share.hesvh.cn/Article/details/gqaanocus.sHtML

wc -l < a.txt
来源：http://mobile.fehbvm.com/Article/details/gtnvkvakk.sHtML

[R43] 按名字查找文件
来源：http://www.share.hesvh.cn/Article/details/gntdlhbgv.sHtML

find . -name "*.log" -type f
来源：http://wap.hesvh.cn/Article/details/gkzaxpqjr.sHtML

[R44] 按修改时间查找
来源：http://baike.fehbvm.com/Article/details/gzzbwgppl.sHtML

find . -mtime -7 -type f
来源：http://blog.fehbvm.com/Article/details/gfmbuibyp.sHtML

[R45] 批量删除
来源：http://www.blog.hesvh.cn/Article/details/gmexxcufq.sHtML

find . -name "*.tmp" -delete
来源：http://wap.zdbjq.cn/Article/details/gwugkypna.sHtML

[R46] 递归替换文件内容
来源：http://www.share.hesvh.cn/Article/details/goctolujd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.zdbjq.cn/Article/details/gjgisetfp.sHtML

[R47] sed 单行替换
来源：http://www.blog.fehbvm.com/Article/details/gdsjbqchl.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fehbvm.com/Article/details/gomkuxwqk.sHtML

[R48] awk 取指定列
来源：http://read.share.hesvh.cn/Article/details/ghgavmnic.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gbnlnjcml.sHtML

[R49] awk 带条件
来源：http://read.share.fehbvm.com/Article/details/gxmxcdydx.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fehbvm.com/Article/details/gbvbzewvv.sHtML

[R50] awk 求和
来源：http://3g.hesvh.cn/Article/details/glchuhdqv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gzxhoixeo.sHtML

[R51] 排序去重取前几
来源：http://m.share.zdbjq.cn/Article/details/gvwazgbky.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fehbvm.com/Article/details/gruunzrwb.sHtML

[R52] 统计行数
来源：http://www.share.hesvh.cn/Article/details/gndwzypfv.sHtML

wc -l a.txt
来源：http://baike.fehbvm.com/Article/details/gxetzzlux.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fehbvm.com/Article/details/gyjqsysii.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.zdbjq.cn/Article/details/gosvjpxpo.sHtML

[R54] 比较两个文件
来源：http://www.share.zdbjq.cn/Article/details/gzxamjclh.sHtML

diff a.txt b.txt
来源：http://www.share.hesvh.cn/Article/details/gzrojzdng.sHtML

[R55] 压缩与解压
来源：http://www.blog.hesvh.cn/Article/details/gsikvehqq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.hesvh.cn/Article/details/gxglocoma.sHtML

[R56] 远程拷贝
来源：http://mobile.hesvh.cn/Article/details/gxdsokiac.sHtML

scp file user@host:/path/
来源：http://read.share.fehbvm.com/Article/details/glxwwbtmm.sHtML

[R57] 远程执行命令
来源：http://mobile.hesvh.cn/Article/details/gggilbecy.sHtML

ssh user@host 'uptime'
来源：http://baike.zdbjq.cn/Article/details/gdnxsqojy.sHtML

[R58] 下载文件
来源：http://wap.fehbvm.com/Article/details/gtvygukog.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.zdbjq.cn/Article/details/gdhrgdoqj.sHtML

[R59] 发 POST JSON
来源：http://blog.zdbjq.cn/Article/details/gvgwxyypk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fehbvm.com/Article/details/ggrjamwvn.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/gkcntdthq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.zdbjq.cn/Article/details/ghxsexddk.sHtML

[R61] 磁盘占用
来源：http://wap.hesvh.cn/Article/details/gtazmqstx.sHtML

df -h;  du -sh *
来源：http://read.share.zdbjq.cn/Article/details/geqkumjqt.sHtML

[R62] 找最占空间的文件
来源：http://read.share.hesvh.cn/Article/details/gurxbigfs.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fehbvm.com/Article/details/gtgacwpne.sHtML

[R63] 内存与进程
来源：http://blog.zdbjq.cn/Article/details/gmyhozdga.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.hesvh.cn/Article/details/gcrynoqhx.sHtML

[R64] 结束进程
来源：http://m.share.fehbvm.com/Article/details/gemqbgjqu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.zdbjq.cn/Article/details/gjlwzyksa.sHtML

[R65] 查看端口占用
来源：http://mobile.hesvh.cn/Article/details/gsiykpjwh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.hesvh.cn/Article/details/gwtlpftrg.sHtML

[R66] 定时任务
来源：http://www.blog.hesvh.cn/Article/details/glldtkhhb.sHtML

crontab -e;  crontab -l
来源：http://blog.hesvh.cn/Article/details/ghldfncop.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.hesvh.cn/Article/details/gwlzouqvc.sHtML

openssl rand -hex 16
来源：http://baike.fehbvm.com/Article/details/ggxmnawns.sHtML

[R68] 计算文件校验值
来源：http://mobile.zdbjq.cn/Article/details/gscboniaa.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fehbvm.com/Article/details/gwekanwzh.sHtML

[R69] 生成随机密码
来源：http://blog.hesvh.cn/Article/details/gvsdcjioi.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.hesvh.cn/Article/details/gtkyktlfa.sHtML

[R70] 时间戳与互转
来源：http://www.blog.hesvh.cn/Article/details/gihjqgdgh.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fehbvm.com/Article/details/gqpqhmthm.sHtML

[R71] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/gkickdrhr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fehbvm.com/Article/details/gnsofnpba.sHtML

[R72] 等待端口就绪
来源：http://baike.zdbjq.cn/Article/details/gjiaritmy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gfevkltpn.sHtML

[R73] 分割大日志
来源：http://m.share.fehbvm.com/Article/details/gakasbkan.sHtML

split -l 1000 big.log part_
来源：http://read.share.fehbvm.com/Article/details/gvbfgltzt.sHtML

[R74] 批量重命名
来源：http://blog.hesvh.cn/Article/details/gltzgnvaj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.hesvh.cn/Article/details/gxqepfpwg.sHtML

[R75] 导出环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/guwdxlmtr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.hesvh.cn/Article/details/ggpxvzejv.sHtML

[R76] 使用临时文件
来源：http://3g.zdbjq.cn/Article/details/gsiomgznb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/gpcwfaguj.sHtML

[R77] 读取用户输入
来源：http://read.share.zdbjq.cn/Article/details/gnjenrrzm.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.zdbjq.cn/Article/details/grqwdohbz.sHtML

[R78] 交互式菜单
来源：http://www.share.fehbvm.com/Article/details/gheetbqyo.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fehbvm.com/Article/details/gsxrmjdjd.sHtML

[R79] 解析命令行选项
来源：http://3g.hesvh.cn/Article/details/gpktgtatc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.hesvh.cn/Article/details/gxopizchh.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.zdbjq.cn/Article/details/gioaxfuaa.sHtML

time ./run.sh
来源：http://www.m.share.fehbvm.com/Article/details/gcrpdfvpb.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gcvwuiadd.sHtML

S. C / C++ 专题
来源：http://m.share.hesvh.cn/Article/details/gtvfoyzvf.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gpmszgyut.sHtML

[S01] C：Hello World
来源：http://read.share.fehbvm.com/Article/details/gapqgvnrv.sHtML

#include <stdio.h>
来源：http://www.share.fehbvm.com/Article/details/gpdxpwaeq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.hesvh.cn/Article/details/gndxtgwqb.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.zdbjq.cn/Article/details/gdodfeofb.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.zdbjq.cn/Article/details/gqtlsrkqr.sHtML

[S03] C：读入整数
来源：http://www.share.hesvh.cn/Article/details/gmcethdqs.sHtML

int x; scanf("%d", &x);
来源：http://m.share.zdbjq.cn/Article/details/gckehguyb.sHtML

[S04] C：字符串复制
来源：http://m.share.fehbvm.com/Article/details/gtqwqtgxo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fehbvm.com/Article/details/gjkrlmhbv.sHtML

[S05] C：字符串长度
来源：http://www.share.fehbvm.com/Article/details/gaqreplup.sHtML

strlen(s)
来源：http://www.blog.hesvh.cn/Article/details/gvbdmwlgm.sHtML

[S06] C：字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/gahsfouar.sHtML

strcmp(a, b) == 0
来源：http://wap.zdbjq.cn/Article/details/gdulbqfvx.sHtML

[S07] C：数组遍历求和
来源：http://baike.hesvh.cn/Article/details/gqjrvmuuz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.zdbjq.cn/Article/details/gcydkujfg.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.zdbjq.cn/Article/details/ggzrzgnwl.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.hesvh.cn/Article/details/gdbilspho.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.zdbjq.cn/Article/details/gdbofahbv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fehbvm.com/Article/details/gycdtyejv.sHtML

[S10] C：指针与解引用
来源：http://baike.zdbjq.cn/Article/details/gnrmruayf.sHtML

int *p = &a;  *p = 5;
来源：http://wap.zdbjq.cn/Article/details/gdampvmik.sHtML

[S11] C：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gwsvgvgvv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.zdbjq.cn/Article/details/gvxjegwph.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fehbvm.com/Article/details/gkkzeyunl.sHtML

fclose(f);
来源：http://wap.fehbvm.com/Article/details/ghjcrmoky.sHtML

[S12] C：写文件
来源：http://www.share.zdbjq.cn/Article/details/ggfutcntw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fehbvm.com/Article/details/ghdsgyvdw.sHtML

[S13] C：宏定义
来源：http://www.m.share.fehbvm.com/Article/details/gbtydhqpe.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fehbvm.com/Article/details/gnpwdrtqk.sHtML

[S14] C：枚举
来源：http://www.blog.fehbvm.com/Article/details/gsbddotew.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.zdbjq.cn/Article/details/gkrtyiitu.sHtML

[S15] C：类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gvgjsxxec.sHtML

(double) a / b
来源：http://baike.hesvh.cn/Article/details/gcnjrhvhc.sHtML

[S16] C：位操作置位
来源：http://m.share.hesvh.cn/Article/details/gjewkotbl.sHtML

x |= (1 << 3);
来源：http://www.share.zdbjq.cn/Article/details/gnqkojrln.sHtML

[S17] C：安全拼接字符串
来源：http://3g.hesvh.cn/Article/details/gindjqhrf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.hesvh.cn/Article/details/gtrbeyuys.sHtML

[S18] C：命令行参数
来源：http://m.share.fehbvm.com/Article/details/grblqgcfn.sHtML

int main(int argc, char **argv)
来源：http://www.share.fehbvm.com/Article/details/gzxzduosw.sHtML

[S19] C：快速排序
来源：http://www.share.hesvh.cn/Article/details/gychymvoc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/gyxugnrjx.sHtML

[S20] C：二分查找
来源：http://wap.hesvh.cn/Article/details/gwnzzxrlw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/gqmaikclw.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.hesvh.cn/Article/details/geyeyomoc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.zdbjq.cn/Article/details/gmqxruomx.sHtML

[S22] C：字符串转数字
来源：http://blog.hesvh.cn/Article/details/glzfvezuw.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.hesvh.cn/Article/details/gnxowoyoi.sHtML

[S23] C：随机数
来源：http://read.share.hesvh.cn/Article/details/gjnodroie.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fehbvm.com/Article/details/ghvjfhsyi.sHtML

[S24] C：获取本地时间
来源：http://read.share.fehbvm.com/Article/details/gfzcyxivz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.zdbjq.cn/Article/details/gxvpausux.sHtML

[S25] C：内存拷贝
来源：http://mobile.zdbjq.cn/Article/details/gvfyzlmfm.sHtML

memcpy(dst, src, n);
来源：http://m.share.hesvh.cn/Article/details/geheemzhi.sHtML

[S26] C：内存清零
来源：http://blog.fehbvm.com/Article/details/gstmvmhej.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.zdbjq.cn/Article/details/gtmmvqmzo.sHtML

[S27] C：定义常量
来源：http://blog.hesvh.cn/Article/details/gpkkncxzt.sHtML

const double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gzniuuhhw.sHtML

[S28] C：静态变量
来源：http://www.share.hesvh.cn/Article/details/gyedlskva.sHtML

static int counter = 0;
来源：http://m.share.fehbvm.com/Article/details/goszyydmm.sHtML

[S29] C：变参函数
来源：http://read.share.fehbvm.com/Article/details/gcuvcepfz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.zdbjq.cn/Article/details/gtaacanrd.sHtML

[S30] C：头文件保护
来源：http://www.m.share.hesvh.cn/Article/details/gegixxaic.sHtML

#ifndef X_H
来源：http://www.share.zdbjq.cn/Article/details/gbvaaiugg.sHtML

#define X_H
来源：http://read.share.fehbvm.com/Article/details/gtdxbrvsa.sHtML

#endif
来源：http://www.blog.zdbjq.cn/Article/details/gpbcuhrzg.sHtML

[S31] C++：Hello World
来源：http://wap.zdbjq.cn/Article/details/gqjdgwpjy.sHtML

#include <iostream>
来源：http://m.share.zdbjq.cn/Article/details/gnitritgv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fehbvm.com/Article/details/gygyiojas.sHtML

[S32] C++：字符串
来源：http://m.share.zdbjq.cn/Article/details/gdqwpiefe.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.hesvh.cn/Article/details/ghbbfnvau.sHtML

[S33] C++：vector 增删
来源：http://www.share.fehbvm.com/Article/details/gylsociqq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.hesvh.cn/Article/details/govpmpbvn.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fehbvm.com/Article/details/glopwowhk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.zdbjq.cn/Article/details/grkbzsxqz.sHtML

[S35] C++：map
来源：http://m.share.fehbvm.com/Article/details/gvstzsuxw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gpppxghdb.sHtML

[S36] C++：unordered_map
来源：http://blog.hesvh.cn/Article/details/gveifyrqf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gthsbnssw.sHtML

[S37] C++：set
来源：http://baike.hesvh.cn/Article/details/gyyckygow.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.hesvh.cn/Article/details/gtlsozosq.sHtML

[S38] C++：排序
来源：http://read.share.fehbvm.com/Article/details/ganfdpins.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.zdbjq.cn/Article/details/gacphqqxf.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.zdbjq.cn/Article/details/gbdmcwuoq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.zdbjq.cn/Article/details/getarvblh.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fehbvm.com/Article/details/ggzcpzavd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.hesvh.cn/Article/details/gnigohffz.sHtML

[S41] C++：类与构造函数
来源：http://mobile.hesvh.cn/Article/details/glzfwvvsr.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fehbvm.com/Article/details/guujkblye.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.hesvh.cn/Article/details/ghdxbqdhw.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.hesvh.cn/Article/details/gesbujfma.sHtML

[S43] C++：智能指针
来源：http://read.share.hesvh.cn/Article/details/gchffyqpx.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fehbvm.com/Article/details/gerfcerxp.sHtML

[S44] C++：引用传参
来源：http://mobile.fehbvm.com/Article/details/gcyebgnti.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.zdbjq.cn/Article/details/gttslhlls.sHtML

[S45] C++：lambda
来源：http://read.share.hesvh.cn/Article/details/gibwhphga.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.hesvh.cn/Article/details/gyfjcwyzs.sHtML

[S46] C++：函数模板
来源：http://3g.zdbjq.cn/Article/details/gbahsenrv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fehbvm.com/Article/details/guohwytkw.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.zdbjq.cn/Article/details/ghobtcldj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.hesvh.cn/Article/details/ghwinujug.sHtML

[S48] C++：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gmekhwhvn.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.hesvh.cn/Article/details/gdysznyym.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fehbvm.com/Article/details/goxhwglzp.sHtML

[S49] C++：写文件
来源：http://read.share.fehbvm.com/Article/details/gjtzfmeey.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.zdbjq.cn/Article/details/gpfbncujf.sHtML

[S50] C++：格式化数字
来源：http://www.share.hesvh.cn/Article/details/gmzcrrwic.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gpawtmegf.sHtML

[S51] C++：显式类型转换
来源：http://blog.fehbvm.com/Article/details/gxpcvqvpp.sHtML

static_cast<double>(a) / b
来源：http://3g.hesvh.cn/Article/details/gdzwjfuyp.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.hesvh.cn/Article/details/gwfokrhua.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fehbvm.com/Article/details/gmreboafh.sHtML

[S53] C++：移动语义
来源：http://mobile.hesvh.cn/Article/details/gxhehqvby.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.hesvh.cn/Article/details/gscqvnbjw.sHtML

[S54] C++：异常处理
来源：http://blog.fehbvm.com/Article/details/gfdiehwnu.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fehbvm.com/Article/details/gvuzkduuc.sHtML

[S55] C++：结构化绑定
来源：http://blog.hesvh.cn/Article/details/gaewtfukm.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.hesvh.cn/Article/details/gphfctmnq.sHtML

[S56] C++：optional
来源：http://www.share.hesvh.cn/Article/details/globooyer.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.hesvh.cn/Article/details/gvalzqhug.sHtML

[S57] C++：编译期常量
来源：http://blog.zdbjq.cn/Article/details/ggosvdblp.sHtML

constexpr int N = 10;
来源：http://read.share.hesvh.cn/Article/details/gknceepbx.sHtML

[S58] C++：命名空间
来源：http://www.share.hesvh.cn/Article/details/ghzmbyxxo.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fehbvm.com/Article/details/gqjmbxspm.sHtML

[S59] C++：静态断言
来源：http://blog.fehbvm.com/Article/details/guokwoaqi.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.hesvh.cn/Article/details/gddrodwey.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fehbvm.com/Article/details/gspxwnkeh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.hesvh.cn/Article/details/ghjskatmy.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gnsniblau.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fehbvm.com/Article/details/grntbvlxs.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gzhwbfgdx.sHtML

[T01] Kotlin：Hello World
来源：http://wap.hesvh.cn/Article/details/goaimhoxb.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gnkmypqtc.sHtML

[T02] Kotlin：变量
来源：http://baike.zdbjq.cn/Article/details/gcxjtyxag.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fehbvm.com/Article/details/gnswxpebk.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fehbvm.com/Article/details/gknrpzkcz.sHtML

"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gacbdxdjb.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.zdbjq.cn/Article/details/gsrbztued.sHtML

val n: String? = null;  n?.length
来源：http://mobile.hesvh.cn/Article/details/gsnoojzxu.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.hesvh.cn/Article/details/gbifdaigs.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fehbvm.com/Article/details/gjpcfnogi.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fehbvm.com/Article/details/gsxgagcbz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fehbvm.com/Article/details/gqfolnspf.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fehbvm.com/Article/details/gzaihtyhy.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.hesvh.cn/Article/details/gpgsuwzqv.sHtML

[T08] Kotlin：数据类
来源：http://www.share.hesvh.cn/Article/details/gqomyxsxv.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fehbvm.com/Article/details/goazmtgcn.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.zdbjq.cn/Article/details/gjdmjbduh.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.zdbjq.cn/Article/details/gjkmfsrtk.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.hesvh.cn/Article/details/garillgff.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.hesvh.cn/Article/details/gfmhjipdv.sHtML


<!-- 参考信息 -->