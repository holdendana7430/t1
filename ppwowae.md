代发 wailian999

readonly PI=3.14
来源：http://wap.zdbjq.cn/Article/details/gkbpdggxm.sHtML

[R04] 位置参数
来源：http://blog.fehbvm.com/Article/details/glaximkxx.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.hesvh.cn/Article/details/ggqapoweb.sHtML

[R05] 参数默认值
来源：http://read.share.hesvh.cn/Article/details/gnmuqncyo.sHtML

name="${1:-default}"
来源：http://mobile.fehbvm.com/Article/details/gfatraedy.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fehbvm.com/Article/details/ghdvhtwkk.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gtgghfgau.sHtML

[R07] if 判断文件
来源：http://baike.hesvh.cn/Article/details/gkdceelmd.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.hesvh.cn/Article/details/gskqvgura.sHtML

[R08] 数值比较
来源：http://3g.hesvh.cn/Article/details/ggrjlekks.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.zdbjq.cn/Article/details/gednbxupv.sHtML

[R09] 字符串比较
来源：http://baike.zdbjq.cn/Article/details/gevcjtexl.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.hesvh.cn/Article/details/grnevlspw.sHtML

[R10] 正则匹配
来源：http://mobile.hesvh.cn/Article/details/gyxdevktf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.zdbjq.cn/Article/details/gsgarivjq.sHtML

[R11] case 多分支
来源：http://www.share.zdbjq.cn/Article/details/gdcijompd.sHtML

case "$1" in
来源：http://mobile.fehbvm.com/Article/details/grarcoxyc.sHtML

start) echo "启动" ;;
来源：http://www.share.zdbjq.cn/Article/details/gcwdcrctx.sHtML

stop)  echo "停止" ;;
来源：http://read.share.hesvh.cn/Article/details/gizjngtfp.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fehbvm.com/Article/details/gjpqikhek.sHtML

esac
来源：http://baike.fehbvm.com/Article/details/gxijvxhbq.sHtML

[R12] for 遍历文件
来源：http://read.share.hesvh.cn/Article/details/gfqilhzhq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.zdbjq.cn/Article/details/gwuldzcsh.sHtML

[R13] for 计数循环
来源：http://www.blog.fehbvm.com/Article/details/ghhuwqzdh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/gyvzmdzvz.sHtML

[R14] C 风格 for
来源：http://m.share.fehbvm.com/Article/details/gellkoiob.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/gktshfuep.sHtML

[R15] while 逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gynausler.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.zdbjq.cn/Article/details/gbpwavpyn.sHtML

[R16] until 等待条件
来源：http://blog.zdbjq.cn/Article/details/gfghvtcxs.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/gspqsbhfr.sHtML

[R17] 数组定义与取值
来源：http://www.share.hesvh.cn/Article/details/gdoecqepo.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fehbvm.com/Article/details/gfyfecygd.sHtML

[R18] 遍历数组
来源：http://baike.hesvh.cn/Article/details/gaarfqege.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.zdbjq.cn/Article/details/gflkiuzce.sHtML

[R19] 数组长度
来源：http://mobile.hesvh.cn/Article/details/gxdyebzkx.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.hesvh.cn/Article/details/gveedqkbz.sHtML

[R20] 关联数组（字典）
来源：http://blog.zdbjq.cn/Article/details/gadjjlzxh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.hesvh.cn/Article/details/gohpdaffg.sHtML

[R21] 字符串长度
来源：http://blog.hesvh.cn/Article/details/gwofdmfbs.sHtML

echo "${#s}"
来源：http://blog.fehbvm.com/Article/details/geonqqkwq.sHtML

[R22] 截取子串
来源：http://mobile.hesvh.cn/Article/details/ghgitwutz.sHtML

echo "${s:0:5}"
来源：http://mobile.hesvh.cn/Article/details/gjkovyazw.sHtML

[R23] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/gzrtjocjh.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fehbvm.com/Article/details/gmfftxdlo.sHtML

[R24] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gscdnyjij.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fehbvm.com/Article/details/guzteeguu.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.hesvh.cn/Article/details/gkhotjnsn.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fehbvm.com/Article/details/gixzxjeym.sHtML

[R26] 命令替换
来源：http://www.share.hesvh.cn/Article/details/gitpoqmpm.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fehbvm.com/Article/details/gutxabfoe.sHtML

[R27] 算术展开
来源：http://read.share.fehbvm.com/Article/details/gucrgswmy.sHtML

echo $((1 + 2 * 3))
来源：http://baike.zdbjq.cn/Article/details/giwbfetfl.sHtML

[R28] 浮点运算
来源：http://wap.fehbvm.com/Article/details/gdwwvxzpl.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.zdbjq.cn/Article/details/gmereykyr.sHtML

[R29] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/gbqudmowr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.zdbjq.cn/Article/details/glfgythqd.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fehbvm.com/Article/details/gxciepfxx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fehbvm.com/Article/details/goycijtjw.sHtML

[R31] 局部变量
来源：http://wap.hesvh.cn/Article/details/gmgghhlkd.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fehbvm.com/Article/details/gzdcuvhwq.sHtML

[R32] 参数个数校验
来源：http://www.blog.zdbjq.cn/Article/details/gxtrocash.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/gvibthdzf.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fehbvm.com/Article/details/gzydobamn.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fehbvm.com/Article/details/gwnuiebik.sHtML

[R34] 退出时清理
来源：http://www.m.share.fehbvm.com/Article/details/gsecbtbrd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gikvizpcm.sHtML

[R35] 后台执行并等待
来源：http://3g.hesvh.cn/Article/details/gghdglwdb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.hesvh.cn/Article/details/gagbiqpzu.sHtML

[R36] 并发执行多个任务
来源：http://baike.zdbjq.cn/Article/details/gqpoqfmug.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.zdbjq.cn/Article/details/gpszggulx.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fehbvm.com/Article/details/gxiuslxjb.sHtML

files=$(ls -1)
来源：http://wap.fehbvm.com/Article/details/guyvmqrvy.sHtML

[R38] 管道串联
来源：http://read.share.zdbjq.cn/Article/details/gggxikzed.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.hesvh.cn/Article/details/gezqvzalg.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.hesvh.cn/Article/details/gawmxbije.sHtML

cmd > out.log 2>&1
来源：http://m.share.hesvh.cn/Article/details/giywvqlzg.sHtML

[R40] 追加写日志
来源：http://baike.fehbvm.com/Article/details/giyeobbek.sHtML

echo "log" >> out.log
来源：http://read.share.hesvh.cn/Article/details/gjghyrblw.sHtML

[R41] 丢弃输出
来源：http://m.share.fehbvm.com/Article/details/grvhthxcw.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fehbvm.com/Article/details/gmkgsbgoi.sHtML

[R42] 输入重定向
来源：http://www.m.share.hesvh.cn/Article/details/guhusozuc.sHtML

wc -l < a.txt
来源：http://blog.fehbvm.com/Article/details/ghriugzvz.sHtML

[R43] 按名字查找文件
来源：http://read.share.fehbvm.com/Article/details/gszstxyiq.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fehbvm.com/Article/details/gfeoslbkv.sHtML

[R44] 按修改时间查找
来源：http://read.share.hesvh.cn/Article/details/gihpnarsd.sHtML

find . -mtime -7 -type f
来源：http://wap.zdbjq.cn/Article/details/grfieifjl.sHtML

[R45] 批量删除
来源：http://blog.hesvh.cn/Article/details/ghfitmcum.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fehbvm.com/Article/details/gkvpuqwql.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fehbvm.com/Article/details/gkktkispw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fehbvm.com/Article/details/gofzyribp.sHtML

[R47] sed 单行替换
来源：http://blog.fehbvm.com/Article/details/givjrnvtu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gffyqknaj.sHtML

[R48] awk 取指定列
来源：http://mobile.zdbjq.cn/Article/details/ghpaixgfn.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.zdbjq.cn/Article/details/ggjimcedc.sHtML

[R49] awk 带条件
来源：http://baike.hesvh.cn/Article/details/gmmhzxvqx.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.zdbjq.cn/Article/details/gavknfmws.sHtML

[R50] awk 求和
来源：http://m.share.hesvh.cn/Article/details/gnrfdmxdg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.zdbjq.cn/Article/details/ghwrydhbf.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fehbvm.com/Article/details/grikbmjbf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.hesvh.cn/Article/details/gsccojock.sHtML

[R52] 统计行数
来源：http://www.share.zdbjq.cn/Article/details/gidueodph.sHtML

wc -l a.txt
来源：http://m.share.fehbvm.com/Article/details/gxhofmxoq.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.hesvh.cn/Article/details/ghkholczj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.zdbjq.cn/Article/details/grkgglcld.sHtML

[R54] 比较两个文件
来源：http://mobile.zdbjq.cn/Article/details/gadjffhvf.sHtML

diff a.txt b.txt
来源：http://wap.zdbjq.cn/Article/details/gvmtfvfml.sHtML

[R55] 压缩与解压
来源：http://blog.zdbjq.cn/Article/details/gpsakmpxz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.hesvh.cn/Article/details/gqoybinro.sHtML

[R56] 远程拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gsumrfhci.sHtML

scp file user@host:/path/
来源：http://baike.fehbvm.com/Article/details/gdyxmrrsm.sHtML

[R57] 远程执行命令
来源：http://blog.hesvh.cn/Article/details/gtvdzrkxl.sHtML

ssh user@host 'uptime'
来源：http://blog.fehbvm.com/Article/details/gkktylyea.sHtML

[R58] 下载文件
来源：http://3g.zdbjq.cn/Article/details/gjibnncmp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.zdbjq.cn/Article/details/gacdhlsvi.sHtML

[R59] 发 POST JSON
来源：http://read.share.hesvh.cn/Article/details/glixdcgdq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fehbvm.com/Article/details/gxsinpbac.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/gzqsihoiz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.hesvh.cn/Article/details/gkdklngvp.sHtML

[R61] 磁盘占用
来源：http://read.share.zdbjq.cn/Article/details/gxczjuyop.sHtML

df -h;  du -sh *
来源：http://mobile.hesvh.cn/Article/details/gqzvklugm.sHtML

[R62] 找最占空间的文件
来源：http://baike.fehbvm.com/Article/details/ghmoiupwe.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.hesvh.cn/Article/details/geztyeuju.sHtML

[R63] 内存与进程
来源：http://www.m.share.hesvh.cn/Article/details/godfyulpv.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.hesvh.cn/Article/details/gdroxoffq.sHtML

[R64] 结束进程
来源：http://read.share.zdbjq.cn/Article/details/gbvxediij.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.zdbjq.cn/Article/details/gppkfiflq.sHtML

[R65] 查看端口占用
来源：http://blog.fehbvm.com/Article/details/gnmmslpna.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.zdbjq.cn/Article/details/glxexucbz.sHtML

[R66] 定时任务
来源：http://wap.zdbjq.cn/Article/details/gzctefsok.sHtML

crontab -e;  crontab -l
来源：http://wap.hesvh.cn/Article/details/gobxfdtwt.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.zdbjq.cn/Article/details/gpnotlyry.sHtML

openssl rand -hex 16
来源：http://mobile.zdbjq.cn/Article/details/gubflhzau.sHtML

[R68] 计算文件校验值
来源：http://blog.zdbjq.cn/Article/details/gutmqfoty.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.hesvh.cn/Article/details/ggsdovysp.sHtML

[R69] 生成随机密码
来源：http://blog.hesvh.cn/Article/details/ghnnvzsfw.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.zdbjq.cn/Article/details/guvbkbtwx.sHtML

[R70] 时间戳与互转
来源：http://read.share.hesvh.cn/Article/details/gjgjicyam.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fehbvm.com/Article/details/gapcvhfiy.sHtML

[R71] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/ghtkggdsf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.hesvh.cn/Article/details/ghwidvabx.sHtML

[R72] 等待端口就绪
来源：http://blog.fehbvm.com/Article/details/gbqjmqmkh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gfbrgddjc.sHtML

[R73] 分割大日志
来源：http://mobile.zdbjq.cn/Article/details/gzgbzkstc.sHtML

split -l 1000 big.log part_
来源：http://www.blog.zdbjq.cn/Article/details/gpdqyecaq.sHtML

[R74] 批量重命名
来源：http://3g.hesvh.cn/Article/details/grcewkmyf.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gyxtawhwj.sHtML

[R75] 导出环境变量
来源：http://blog.zdbjq.cn/Article/details/gtevknxso.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.zdbjq.cn/Article/details/gofpxrrpv.sHtML

[R76] 使用临时文件
来源：http://mobile.zdbjq.cn/Article/details/gsspidpng.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/ggwdisnef.sHtML

[R77] 读取用户输入
来源：http://3g.hesvh.cn/Article/details/gawuqqocr.sHtML

read -rp "请输入: " ans
来源：http://baike.zdbjq.cn/Article/details/gerymnhcc.sHtML

[R78] 交互式菜单
来源：http://www.blog.zdbjq.cn/Article/details/gezxsqwrw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.hesvh.cn/Article/details/gxirvmbql.sHtML

[R79] 解析命令行选项
来源：http://read.share.hesvh.cn/Article/details/gpilvmsyz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.hesvh.cn/Article/details/gyjwbkaij.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.hesvh.cn/Article/details/gvtjbegai.sHtML

time ./run.sh
来源：http://blog.zdbjq.cn/Article/details/ggqhlynhf.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gqbgrxovv.sHtML

S. C / C++ 专题
来源：http://www.blog.fehbvm.com/Article/details/gfudgrcqm.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ghtniatgj.sHtML

[S01] C：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gvimasrqz.sHtML

#include <stdio.h>
来源：http://m.share.fehbvm.com/Article/details/gjbqzvdcl.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fehbvm.com/Article/details/gerjyskpv.sHtML

[S02] C：变量与格式化输出
来源：http://blog.zdbjq.cn/Article/details/gnsntsfxm.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.hesvh.cn/Article/details/gyftytoyd.sHtML

[S03] C：读入整数
来源：http://www.blog.zdbjq.cn/Article/details/gersfzdjd.sHtML

int x; scanf("%d", &x);
来源：http://wap.hesvh.cn/Article/details/gmbazqyov.sHtML

[S04] C：字符串复制
来源：http://www.blog.hesvh.cn/Article/details/gresxcwvt.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.zdbjq.cn/Article/details/greloitnu.sHtML

[S05] C：字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/gcqxtbwrq.sHtML

strlen(s)
来源：http://baike.hesvh.cn/Article/details/gdatpkrjb.sHtML

[S06] C：字符串比较
来源：http://blog.fehbvm.com/Article/details/glzmaepgr.sHtML

strcmp(a, b) == 0
来源：http://baike.hesvh.cn/Article/details/gticwmkhs.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fehbvm.com/Article/details/gcbggbgeo.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.zdbjq.cn/Article/details/glxminxkt.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.hesvh.cn/Article/details/gkgjmbfeo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.hesvh.cn/Article/details/gipfcnaxe.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.hesvh.cn/Article/details/gwebpmipr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fehbvm.com/Article/details/gqpgkieqk.sHtML

[S10] C：指针与解引用
来源：http://baike.fehbvm.com/Article/details/gshuahngb.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.zdbjq.cn/Article/details/glnxlzyjc.sHtML

[S11] C：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/glnfhvulf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.hesvh.cn/Article/details/gzrjkxmeo.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.hesvh.cn/Article/details/gmtawzynk.sHtML

fclose(f);
来源：http://m.share.fehbvm.com/Article/details/gqadusufx.sHtML

[S12] C：写文件
来源：http://m.share.fehbvm.com/Article/details/gfopbnqiz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.zdbjq.cn/Article/details/gjvzhwysc.sHtML

[S13] C：宏定义
来源：http://www.blog.fehbvm.com/Article/details/gxfcdjsdr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.hesvh.cn/Article/details/gwcmpdxnh.sHtML

[S14] C：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/ghgmvyssf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.zdbjq.cn/Article/details/ghmlhuuob.sHtML

[S15] C：类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gfqoqeurt.sHtML

(double) a / b
来源：http://baike.zdbjq.cn/Article/details/grkqnonya.sHtML

[S16] C：位操作置位
来源：http://wap.zdbjq.cn/Article/details/gsruowmnf.sHtML

x |= (1 << 3);
来源：http://blog.fehbvm.com/Article/details/gpeocmttv.sHtML

[S17] C：安全拼接字符串
来源：http://3g.hesvh.cn/Article/details/ghvhkohvu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.hesvh.cn/Article/details/gexcxccqb.sHtML

[S18] C：命令行参数
来源：http://www.share.zdbjq.cn/Article/details/gqfudjcxq.sHtML

int main(int argc, char **argv)
来源：http://baike.zdbjq.cn/Article/details/gsiaewhau.sHtML

[S19] C：快速排序
来源：http://wap.fehbvm.com/Article/details/gzozpbsyd.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/gxwigrtks.sHtML

[S20] C：二分查找
来源：http://www.blog.fehbvm.com/Article/details/gatnprurp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gyszzqujv.sHtML

[S21] C：字符类别判断
来源：http://www.share.hesvh.cn/Article/details/gudjqoxeq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.zdbjq.cn/Article/details/gmbrckujs.sHtML

[S22] C：字符串转数字
来源：http://3g.hesvh.cn/Article/details/gvnnhhjal.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fehbvm.com/Article/details/gpirwxznl.sHtML

[S23] C：随机数
来源：http://read.share.zdbjq.cn/Article/details/gsjgyxkrw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.zdbjq.cn/Article/details/gyucpknlq.sHtML

[S24] C：获取本地时间
来源：http://wap.fehbvm.com/Article/details/gyiikegnj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.hesvh.cn/Article/details/gtkjpseym.sHtML

[S25] C：内存拷贝
来源：http://baike.fehbvm.com/Article/details/gebrgofhu.sHtML

memcpy(dst, src, n);
来源：http://www.blog.hesvh.cn/Article/details/gzddykppm.sHtML

[S26] C：内存清零
来源：http://3g.zdbjq.cn/Article/details/gogxvathr.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fehbvm.com/Article/details/gmxydvikm.sHtML

[S27] C：定义常量
来源：http://www.share.hesvh.cn/Article/details/gfjnyxcau.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gspixmpav.sHtML

[S28] C：静态变量
来源：http://wap.hesvh.cn/Article/details/gxzwtttli.sHtML

static int counter = 0;
来源：http://www.blog.fehbvm.com/Article/details/gbdpqoelk.sHtML

[S29] C：变参函数
来源：http://www.m.share.fehbvm.com/Article/details/gvgksjlgz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.hesvh.cn/Article/details/glhmwrkhe.sHtML

[S30] C：头文件保护
来源：http://wap.fehbvm.com/Article/details/grawccitk.sHtML

#ifndef X_H
来源：http://www.blog.zdbjq.cn/Article/details/gmpclihef.sHtML

#define X_H
来源：http://www.share.hesvh.cn/Article/details/gldhjvkhk.sHtML

#endif
来源：http://read.share.hesvh.cn/Article/details/gokmwjeiq.sHtML

[S31] C++：Hello World
来源：http://3g.zdbjq.cn/Article/details/gnrkcifpo.sHtML

#include <iostream>
来源：http://www.blog.hesvh.cn/Article/details/gwjnrdiss.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fehbvm.com/Article/details/gyfnatgab.sHtML

[S32] C++：字符串
来源：http://blog.hesvh.cn/Article/details/gcuanvaal.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.zdbjq.cn/Article/details/gllqozvvj.sHtML

[S33] C++：vector 增删
来源：http://wap.zdbjq.cn/Article/details/gadzfoxed.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.zdbjq.cn/Article/details/gmjqpukqn.sHtML

[S34] C++：遍历 vector
来源：http://wap.hesvh.cn/Article/details/gffjaqrge.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.zdbjq.cn/Article/details/gqdhlixaq.sHtML

[S35] C++：map
来源：http://www.m.share.hesvh.cn/Article/details/gbqusiibc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gekdcnkcn.sHtML

[S36] C++：unordered_map
来源：http://m.share.hesvh.cn/Article/details/grplbvclg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/ggctwxtjm.sHtML

[S37] C++：set
来源：http://baike.fehbvm.com/Article/details/gurkfzhlg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.hesvh.cn/Article/details/gtxmnbsne.sHtML

[S38] C++：排序
来源：http://www.blog.zdbjq.cn/Article/details/gltyygrsl.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fehbvm.com/Article/details/gwitioqxw.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.hesvh.cn/Article/details/glqmzbtuy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.zdbjq.cn/Article/details/gggwjfypy.sHtML

[S40] C++：查找元素
来源：http://mobile.fehbvm.com/Article/details/gwheqbdrr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.hesvh.cn/Article/details/gexhnzxcv.sHtML

[S41] C++：类与构造函数
来源：http://wap.zdbjq.cn/Article/details/giueziblq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.zdbjq.cn/Article/details/gcynccvzt.sHtML

[S42] C++：继承与虚函数
来源：http://baike.zdbjq.cn/Article/details/gqbyxkajr.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.hesvh.cn/Article/details/ggnblcoon.sHtML

[S43] C++：智能指针
来源：http://www.share.zdbjq.cn/Article/details/glbqcfwnc.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.hesvh.cn/Article/details/ggbsnrzrj.sHtML

[S44] C++：引用传参
来源：http://blog.hesvh.cn/Article/details/gajrpygfk.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fehbvm.com/Article/details/grdwqmsgd.sHtML

[S45] C++：lambda
来源：http://m.share.hesvh.cn/Article/details/gstlopezh.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fehbvm.com/Article/details/ggjmqixep.sHtML

[S46] C++：函数模板
来源：http://mobile.zdbjq.cn/Article/details/gcpxfmoor.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.zdbjq.cn/Article/details/gnmbrzuim.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.zdbjq.cn/Article/details/gsfxyjwsl.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.hesvh.cn/Article/details/glrsrtmsi.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gonzexots.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.zdbjq.cn/Article/details/gonrbanto.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gtmjezaqo.sHtML

[S49] C++：写文件
来源：http://read.share.zdbjq.cn/Article/details/gpmetnhmn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.hesvh.cn/Article/details/gqrlryklm.sHtML

[S50] C++：格式化数字
来源：http://3g.fehbvm.com/Article/details/gbwsrxona.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gzhhuqhpn.sHtML

[S51] C++：显式类型转换
来源：http://read.share.zdbjq.cn/Article/details/ghsyrcqut.sHtML

static_cast<double>(a) / b
来源：http://3g.fehbvm.com/Article/details/gmdwyudkz.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fehbvm.com/Article/details/gotyhouwm.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.hesvh.cn/Article/details/gffdlqcit.sHtML

[S53] C++：移动语义
来源：http://mobile.fehbvm.com/Article/details/gfcxirobi.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.zdbjq.cn/Article/details/gfywcvnel.sHtML

[S54] C++：异常处理
来源：http://m.share.hesvh.cn/Article/details/gqqpnldsu.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.hesvh.cn/Article/details/gwqnvfehx.sHtML

[S55] C++：结构化绑定
来源：http://blog.hesvh.cn/Article/details/grgcravyo.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fehbvm.com/Article/details/gdxwvnana.sHtML

[S56] C++：optional
来源：http://mobile.fehbvm.com/Article/details/gzdiwmdek.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.hesvh.cn/Article/details/grpjmczms.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.hesvh.cn/Article/details/gdoifehtp.sHtML

constexpr int N = 10;
来源：http://3g.hesvh.cn/Article/details/gvohklszf.sHtML

[S58] C++：命名空间
来源：http://baike.zdbjq.cn/Article/details/gjqfiyixy.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fehbvm.com/Article/details/goohzkpkl.sHtML

[S59] C++：静态断言
来源：http://blog.zdbjq.cn/Article/details/gqeexmxic.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.hesvh.cn/Article/details/gtphxrjui.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fehbvm.com/Article/details/gllhrwegs.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.hesvh.cn/Article/details/gncylmtox.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gzfvvdxin.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.hesvh.cn/Article/details/giomhjnad.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gnketlakx.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fehbvm.com/Article/details/gsqpkskuw.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/gfeidivwz.sHtML

[T02] Kotlin：变量
来源：http://3g.hesvh.cn/Article/details/gqimcdpwe.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.zdbjq.cn/Article/details/gzecjaafs.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.hesvh.cn/Article/details/grwjtesee.sHtML

"值: $b"
来源：http://3g.fehbvm.com/Article/details/gqdwxcsgl.sHtML

[T04] Kotlin：空安全
来源：http://baike.zdbjq.cn/Article/details/gzypkeuuz.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fehbvm.com/Article/details/goozdjeju.sHtML


<!-- 参考信息 -->