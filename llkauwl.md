代发 wailian999

readonly PI=3.14
来源：http://m.share.fehbvm.com/Article/details/gyayhbbwg.sHtML

[R04] 位置参数
来源：http://mobile.zdbjq.cn/Article/details/ghksgeusa.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fehbvm.com/Article/details/gpdvbyqwh.sHtML

[R05] 参数默认值
来源：http://www.m.share.zdbjq.cn/Article/details/ghclsemel.sHtML

name="${1:-default}"
来源：http://read.share.zdbjq.cn/Article/details/gfsiurjhq.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fehbvm.com/Article/details/gmgyxodow.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/gaxdzxokr.sHtML

[R07] if 判断文件
来源：http://mobile.hesvh.cn/Article/details/gjhjzddju.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gffcgvjtm.sHtML

[R08] 数值比较
来源：http://blog.fehbvm.com/Article/details/gjizhdwkr.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gwmannkiw.sHtML

[R09] 字符串比较
来源：http://3g.hesvh.cn/Article/details/gsauuxqzb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fehbvm.com/Article/details/gtswrdljz.sHtML

[R10] 正则匹配
来源：http://blog.zdbjq.cn/Article/details/glvpwvhcz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fehbvm.com/Article/details/gjqevzulh.sHtML

[R11] case 多分支
来源：http://wap.hesvh.cn/Article/details/ghznnryal.sHtML

case "$1" in
来源：http://read.share.hesvh.cn/Article/details/gmottcgur.sHtML

start) echo "启动" ;;
来源：http://baike.fehbvm.com/Article/details/guryuppzz.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gpnpstpkp.sHtML

*)     echo "未知命令" ;;
来源：http://wap.hesvh.cn/Article/details/gknapalrv.sHtML

esac
来源：http://read.share.zdbjq.cn/Article/details/gqriafqvd.sHtML

[R12] for 遍历文件
来源：http://www.m.share.zdbjq.cn/Article/details/gvvfmvpbp.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fehbvm.com/Article/details/gmjjawvbm.sHtML

[R13] for 计数循环
来源：http://www.m.share.zdbjq.cn/Article/details/gwkybvkqk.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/gconogvjc.sHtML

[R14] C 风格 for
来源：http://read.share.fehbvm.com/Article/details/guskhjgcv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/ghcpivsyi.sHtML

[R15] while 逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gklhmnmix.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.hesvh.cn/Article/details/gvimljtqi.sHtML

[R16] until 等待条件
来源：http://read.share.fehbvm.com/Article/details/ggjievmdu.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gdbkvarvz.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fehbvm.com/Article/details/gvxdhymbf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.zdbjq.cn/Article/details/grovhvzpd.sHtML

[R18] 遍历数组
来源：http://m.share.hesvh.cn/Article/details/gcghikumt.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.hesvh.cn/Article/details/gssomgivt.sHtML

[R19] 数组长度
来源：http://mobile.hesvh.cn/Article/details/gullzydcv.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gqzlyjmag.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.zdbjq.cn/Article/details/gzfqqwasl.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.hesvh.cn/Article/details/gfxhbxcxl.sHtML

[R21] 字符串长度
来源：http://baike.zdbjq.cn/Article/details/ghpdeqpex.sHtML

echo "${#s}"
来源：http://baike.hesvh.cn/Article/details/gtjnihroy.sHtML

[R22] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/gqoflbecd.sHtML

echo "${s:0:5}"
来源：http://www.share.zdbjq.cn/Article/details/gwnbsqnsy.sHtML

[R23] 字符串替换
来源：http://baike.zdbjq.cn/Article/details/gkfhmuiro.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.zdbjq.cn/Article/details/gavpiopju.sHtML

[R24] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/geqbsivfo.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.hesvh.cn/Article/details/gxzikrluy.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.hesvh.cn/Article/details/gqeevsgyr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.hesvh.cn/Article/details/gsgauelyw.sHtML

[R26] 命令替换
来源：http://www.blog.hesvh.cn/Article/details/gdpbkihej.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.zdbjq.cn/Article/details/gokdqltnr.sHtML

[R27] 算术展开
来源：http://m.share.zdbjq.cn/Article/details/gxfshdrme.sHtML

echo $((1 + 2 * 3))
来源：http://blog.zdbjq.cn/Article/details/gffxznexm.sHtML

[R28] 浮点运算
来源：http://www.share.fehbvm.com/Article/details/gziwbozls.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fehbvm.com/Article/details/gfkqtwyjn.sHtML

[R29] 定义函数
来源：http://wap.hesvh.cn/Article/details/grccvxiqm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.hesvh.cn/Article/details/gpulrslmn.sHtML

[R30] 函数返回状态码
来源：http://mobile.zdbjq.cn/Article/details/gmwbwjirz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.zdbjq.cn/Article/details/gsfnqhhyt.sHtML

[R31] 局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gyyyovrnh.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fehbvm.com/Article/details/gpbyadfyz.sHtML

[R32] 参数个数校验
来源：http://blog.fehbvm.com/Article/details/gvbmwipoi.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gonzkbqdy.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.zdbjq.cn/Article/details/gouxwlgba.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.zdbjq.cn/Article/details/gwsylurol.sHtML

[R34] 退出时清理
来源：http://www.m.share.hesvh.cn/Article/details/gdftmlkik.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/gwrobhmhm.sHtML

[R35] 后台执行并等待
来源：http://m.share.hesvh.cn/Article/details/gbzxepobg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.hesvh.cn/Article/details/gkstnvfpu.sHtML

[R36] 并发执行多个任务
来源：http://www.share.hesvh.cn/Article/details/gzgoylikr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.hesvh.cn/Article/details/goxjnquvy.sHtML

[R37] 把输出赋给变量
来源：http://mobile.hesvh.cn/Article/details/gqxycxtyl.sHtML

files=$(ls -1)
来源：http://read.share.fehbvm.com/Article/details/gbcsbdmud.sHtML

[R38] 管道串联
来源：http://www.share.fehbvm.com/Article/details/gqirmoawp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fehbvm.com/Article/details/gdmtomjkr.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.zdbjq.cn/Article/details/gxrjygogm.sHtML

cmd > out.log 2>&1
来源：http://www.blog.hesvh.cn/Article/details/gdckqlsqs.sHtML

[R40] 追加写日志
来源：http://read.share.hesvh.cn/Article/details/gbpguxuyt.sHtML

echo "log" >> out.log
来源：http://www.share.fehbvm.com/Article/details/gmfkrzbjt.sHtML

[R41] 丢弃输出
来源：http://3g.fehbvm.com/Article/details/gfbfrdqbb.sHtML

cmd >/dev/null 2>&1
来源：http://3g.zdbjq.cn/Article/details/gnnnuiwzh.sHtML

[R42] 输入重定向
来源：http://baike.fehbvm.com/Article/details/gkylnsxmi.sHtML

wc -l < a.txt
来源：http://www.share.hesvh.cn/Article/details/gtspyjfog.sHtML

[R43] 按名字查找文件
来源：http://read.share.fehbvm.com/Article/details/gezarrsii.sHtML

find . -name "*.log" -type f
来源：http://www.share.hesvh.cn/Article/details/gpeecrkai.sHtML

[R44] 按修改时间查找
来源：http://wap.fehbvm.com/Article/details/gxhaxkitk.sHtML

find . -mtime -7 -type f
来源：http://3g.fehbvm.com/Article/details/guivztdkf.sHtML

[R45] 批量删除
来源：http://wap.fehbvm.com/Article/details/gtsifxutk.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.zdbjq.cn/Article/details/gcpnhleoe.sHtML

[R46] 递归替换文件内容
来源：http://m.share.hesvh.cn/Article/details/glhpvwbrh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fehbvm.com/Article/details/gxiehkaup.sHtML

[R47] sed 单行替换
来源：http://www.share.hesvh.cn/Article/details/gtkfbumtm.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.zdbjq.cn/Article/details/gynwrgpbb.sHtML

[R48] awk 取指定列
来源：http://wap.hesvh.cn/Article/details/gzvjezsot.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.hesvh.cn/Article/details/gaqcigsob.sHtML

[R49] awk 带条件
来源：http://m.share.zdbjq.cn/Article/details/gpfrnflqq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.hesvh.cn/Article/details/gxjevuvlp.sHtML

[R50] awk 求和
来源：http://www.m.share.zdbjq.cn/Article/details/grpvjayep.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gucigohmb.sHtML

[R51] 排序去重取前几
来源：http://blog.zdbjq.cn/Article/details/grizkxspt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fehbvm.com/Article/details/grebvzkpb.sHtML

[R52] 统计行数
来源：http://www.m.share.fehbvm.com/Article/details/gycqutfdz.sHtML

wc -l a.txt
来源：http://read.share.fehbvm.com/Article/details/gwzxmdfnb.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.hesvh.cn/Article/details/gerrrupms.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.hesvh.cn/Article/details/gqzbguupd.sHtML

[R54] 比较两个文件
来源：http://www.share.hesvh.cn/Article/details/gaqcixyqs.sHtML

diff a.txt b.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gloqwcvnn.sHtML

[R55] 压缩与解压
来源：http://blog.hesvh.cn/Article/details/gwzftiokj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fehbvm.com/Article/details/gzvgbtemj.sHtML

[R56] 远程拷贝
来源：http://read.share.zdbjq.cn/Article/details/gzswaefcq.sHtML

scp file user@host:/path/
来源：http://3g.hesvh.cn/Article/details/gfztynjfi.sHtML

[R57] 远程执行命令
来源：http://www.m.share.hesvh.cn/Article/details/grcamndrl.sHtML

ssh user@host 'uptime'
来源：http://m.share.fehbvm.com/Article/details/gzhaqbocs.sHtML

[R58] 下载文件
来源：http://www.share.zdbjq.cn/Article/details/glbbjnqsc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fehbvm.com/Article/details/gcjojczho.sHtML

[R59] 发 POST JSON
来源：http://www.share.fehbvm.com/Article/details/gkzwzhznh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.zdbjq.cn/Article/details/gthyetrbe.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/gvmcfeurh.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fehbvm.com/Article/details/gylofzkyf.sHtML

[R61] 磁盘占用
来源：http://www.blog.hesvh.cn/Article/details/goquxikmc.sHtML

df -h;  du -sh *
来源：http://blog.zdbjq.cn/Article/details/gdlkzdosi.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fehbvm.com/Article/details/ggijzfyog.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fehbvm.com/Article/details/gaqzifrys.sHtML

[R63] 内存与进程
来源：http://wap.fehbvm.com/Article/details/gqefaiojs.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.hesvh.cn/Article/details/gmovjjnnu.sHtML

[R64] 结束进程
来源：http://www.m.share.hesvh.cn/Article/details/gbsgchkvd.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.hesvh.cn/Article/details/gfdgyzykt.sHtML

[R65] 查看端口占用
来源：http://m.share.zdbjq.cn/Article/details/gpkecvnuc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.hesvh.cn/Article/details/gypsqnjdf.sHtML

[R66] 定时任务
来源：http://www.blog.hesvh.cn/Article/details/gqbsrlfpj.sHtML

crontab -e;  crontab -l
来源：http://www.share.fehbvm.com/Article/details/geljaduvo.sHtML

[R67] 生成随机十六进制串
来源：http://blog.hesvh.cn/Article/details/gfwrjhprp.sHtML

openssl rand -hex 16
来源：http://www.share.fehbvm.com/Article/details/grxentarg.sHtML

[R68] 计算文件校验值
来源：http://baike.fehbvm.com/Article/details/gyglscsfz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.hesvh.cn/Article/details/gqiylsboj.sHtML

[R69] 生成随机密码
来源：http://www.m.share.zdbjq.cn/Article/details/gqtujobdm.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fehbvm.com/Article/details/gjpvzbksr.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.hesvh.cn/Article/details/gmwggncex.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.zdbjq.cn/Article/details/gcngwtuxu.sHtML

[R71] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gamjqtuti.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.zdbjq.cn/Article/details/gjmmqyvbu.sHtML

[R72] 等待端口就绪
来源：http://www.share.hesvh.cn/Article/details/gtvxnjrte.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/getsipnvf.sHtML

[R73] 分割大日志
来源：http://wap.hesvh.cn/Article/details/gqfdfvxgg.sHtML

split -l 1000 big.log part_
来源：http://www.blog.zdbjq.cn/Article/details/ghlpcdmbc.sHtML

[R74] 批量重命名
来源：http://www.share.fehbvm.com/Article/details/ghdtrrjdk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fehbvm.com/Article/details/gfiulybkz.sHtML

[R75] 导出环境变量
来源：http://blog.hesvh.cn/Article/details/gnksjuhkb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.zdbjq.cn/Article/details/gsxehxhpk.sHtML

[R76] 使用临时文件
来源：http://blog.fehbvm.com/Article/details/gfwrccqrq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gbzjhzfdn.sHtML

[R77] 读取用户输入
来源：http://blog.fehbvm.com/Article/details/gyaqzjcyo.sHtML

read -rp "请输入: " ans
来源：http://www.share.fehbvm.com/Article/details/gsuwlbumj.sHtML

[R78] 交互式菜单
来源：http://www.blog.hesvh.cn/Article/details/guaxqscvk.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.zdbjq.cn/Article/details/gydqpxlyn.sHtML

[R79] 解析命令行选项
来源：http://m.share.zdbjq.cn/Article/details/gbgxuaean.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.zdbjq.cn/Article/details/gtkzccfux.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.hesvh.cn/Article/details/gnioghklg.sHtML

time ./run.sh
来源：http://wap.hesvh.cn/Article/details/gjkieiani.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gaxqzvrsk.sHtML

S. C / C++ 专题
来源：http://www.blog.hesvh.cn/Article/details/gvlrjvcqg.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gtubiaspx.sHtML

[S01] C：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gaayrkndf.sHtML

#include <stdio.h>
来源：http://baike.fehbvm.com/Article/details/gjptqoyff.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.zdbjq.cn/Article/details/geotaghow.sHtML

[S02] C：变量与格式化输出
来源：http://baike.zdbjq.cn/Article/details/gbqwdhlex.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.hesvh.cn/Article/details/gzunrlxlc.sHtML

[S03] C：读入整数
来源：http://wap.hesvh.cn/Article/details/gnnfugzjl.sHtML

int x; scanf("%d", &x);
来源：http://read.share.zdbjq.cn/Article/details/gxcgyxziy.sHtML

[S04] C：字符串复制
来源：http://blog.fehbvm.com/Article/details/goijyiijk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.hesvh.cn/Article/details/gulpsymdv.sHtML

[S05] C：字符串长度
来源：http://mobile.zdbjq.cn/Article/details/gclezpkqg.sHtML

strlen(s)
来源：http://3g.hesvh.cn/Article/details/gaeqctohc.sHtML

[S06] C：字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gnvmrzjte.sHtML

strcmp(a, b) == 0
来源：http://read.share.fehbvm.com/Article/details/gugzfhxlj.sHtML

[S07] C：数组遍历求和
来源：http://wap.hesvh.cn/Article/details/grhnrozzt.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.zdbjq.cn/Article/details/gsldjgmst.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.zdbjq.cn/Article/details/gzpfalabe.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.zdbjq.cn/Article/details/gnlveiagb.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fehbvm.com/Article/details/gnirfoemy.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.zdbjq.cn/Article/details/ggjpexvqa.sHtML

[S10] C：指针与解引用
来源：http://3g.zdbjq.cn/Article/details/giuafgdpr.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.zdbjq.cn/Article/details/grqwlysci.sHtML

[S11] C：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gaysjbxxu.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fehbvm.com/Article/details/goxcqpevq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.hesvh.cn/Article/details/gkkofxabu.sHtML

fclose(f);
来源：http://read.share.hesvh.cn/Article/details/gyjioyvza.sHtML

[S12] C：写文件
来源：http://3g.hesvh.cn/Article/details/gjnxabhjx.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.hesvh.cn/Article/details/galwttvnt.sHtML

[S13] C：宏定义
来源：http://mobile.fehbvm.com/Article/details/gmjljhpcg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.hesvh.cn/Article/details/ghvrosbnb.sHtML

[S14] C：枚举
来源：http://www.share.fehbvm.com/Article/details/gskkriaqo.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.hesvh.cn/Article/details/gpzzzcdog.sHtML

[S15] C：类型转换
来源：http://www.share.zdbjq.cn/Article/details/grkkgyvjh.sHtML

(double) a / b
来源：http://read.share.fehbvm.com/Article/details/gtclvukic.sHtML

[S16] C：位操作置位
来源：http://www.m.share.hesvh.cn/Article/details/gcnwjsfzz.sHtML

x |= (1 << 3);
来源：http://www.share.zdbjq.cn/Article/details/gyfmikpwb.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gzsjhaxni.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fehbvm.com/Article/details/gxzjseiyp.sHtML

[S18] C：命令行参数
来源：http://wap.fehbvm.com/Article/details/gjgqrnjsq.sHtML

int main(int argc, char **argv)
来源：http://mobile.hesvh.cn/Article/details/golthyhzl.sHtML

[S19] C：快速排序
来源：http://mobile.fehbvm.com/Article/details/gpnbntspf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/ggoghzyrp.sHtML

[S20] C：二分查找
来源：http://read.share.zdbjq.cn/Article/details/gyivdboco.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/gstsaogcj.sHtML

[S21] C：字符类别判断
来源：http://blog.fehbvm.com/Article/details/guciugvop.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.hesvh.cn/Article/details/gobqwijoi.sHtML

[S22] C：字符串转数字
来源：http://m.share.fehbvm.com/Article/details/gdkzhavzd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fehbvm.com/Article/details/gqfokdrix.sHtML

[S23] C：随机数
来源：http://3g.zdbjq.cn/Article/details/gtzlpklzs.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.zdbjq.cn/Article/details/gnadmkwgv.sHtML

[S24] C：获取本地时间
来源：http://mobile.hesvh.cn/Article/details/giclxgfgc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.zdbjq.cn/Article/details/glnumtmzq.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/ggsvurnst.sHtML

memcpy(dst, src, n);
来源：http://www.share.fehbvm.com/Article/details/gqzsizsna.sHtML

[S26] C：内存清零
来源：http://read.share.zdbjq.cn/Article/details/grhjdburu.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fehbvm.com/Article/details/gibiupaiv.sHtML

[S27] C：定义常量
来源：http://m.share.zdbjq.cn/Article/details/gxbtsgghi.sHtML

const double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gciuzexqk.sHtML

[S28] C：静态变量
来源：http://wap.fehbvm.com/Article/details/gzovzxbtv.sHtML

static int counter = 0;
来源：http://read.share.fehbvm.com/Article/details/gbxtyncwl.sHtML

[S29] C：变参函数
来源：http://www.share.zdbjq.cn/Article/details/gpbjnrayd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fehbvm.com/Article/details/grkhjvtvj.sHtML

[S30] C：头文件保护
来源：http://read.share.fehbvm.com/Article/details/gpdojjgqp.sHtML

#ifndef X_H
来源：http://3g.hesvh.cn/Article/details/gnhogdwmx.sHtML

#define X_H
来源：http://www.blog.zdbjq.cn/Article/details/gllrtgvva.sHtML

#endif
来源：http://www.blog.hesvh.cn/Article/details/giscuqiat.sHtML

[S31] C++：Hello World
来源：http://blog.fehbvm.com/Article/details/gcrhxxhrk.sHtML

#include <iostream>
来源：http://baike.hesvh.cn/Article/details/guzpenqvb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.hesvh.cn/Article/details/geirtnaqg.sHtML

[S32] C++：字符串
来源：http://wap.fehbvm.com/Article/details/guutnocsl.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.zdbjq.cn/Article/details/gftnowcfo.sHtML

[S33] C++：vector 增删
来源：http://m.share.fehbvm.com/Article/details/gcqxafbxl.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.zdbjq.cn/Article/details/gaakmzkrc.sHtML

[S34] C++：遍历 vector
来源：http://baike.hesvh.cn/Article/details/gabhwxtke.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.hesvh.cn/Article/details/gncymywvp.sHtML

[S35] C++：map
来源：http://m.share.fehbvm.com/Article/details/gzbuwlfap.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/gqzvwsgha.sHtML

[S36] C++：unordered_map
来源：http://wap.zdbjq.cn/Article/details/gjumwxruu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fehbvm.com/Article/details/geaymhehj.sHtML

[S37] C++：set
来源：http://baike.fehbvm.com/Article/details/gvxpsbsyg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.hesvh.cn/Article/details/gflcrgavt.sHtML

[S38] C++：排序
来源：http://www.blog.zdbjq.cn/Article/details/gndggdzcn.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/gqykzgooo.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.hesvh.cn/Article/details/gxuygjodf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fehbvm.com/Article/details/gjjomycnp.sHtML

[S40] C++：查找元素
来源：http://baike.hesvh.cn/Article/details/gevdmbkat.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.hesvh.cn/Article/details/gmybizwwb.sHtML

[S41] C++：类与构造函数
来源：http://baike.fehbvm.com/Article/details/ggvfgrdga.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fehbvm.com/Article/details/ggioymfoe.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.zdbjq.cn/Article/details/gitpwfdih.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fehbvm.com/Article/details/grqzchdqr.sHtML

[S43] C++：智能指针
来源：http://wap.fehbvm.com/Article/details/grgouwame.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.zdbjq.cn/Article/details/gyvcpjjgi.sHtML

[S44] C++：引用传参
来源：http://blog.hesvh.cn/Article/details/gqjotblfe.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gaaxaqmbq.sHtML

[S45] C++：lambda
来源：http://3g.hesvh.cn/Article/details/gkxkykqbx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fehbvm.com/Article/details/geeutwrid.sHtML

[S46] C++：函数模板
来源：http://mobile.hesvh.cn/Article/details/gulpdcsvg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fehbvm.com/Article/details/gwbqgjgri.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.zdbjq.cn/Article/details/gmiugspiu.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.zdbjq.cn/Article/details/gryuzfauf.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/giqkdzxwp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.hesvh.cn/Article/details/gfckmoxlw.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.zdbjq.cn/Article/details/ginmbzhmh.sHtML

[S49] C++：写文件
来源：http://www.share.hesvh.cn/Article/details/gjhzpnxbc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.zdbjq.cn/Article/details/gupnkfbpv.sHtML

[S50] C++：格式化数字
来源：http://blog.fehbvm.com/Article/details/gobzdivme.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gazhvkiww.sHtML

[S51] C++：显式类型转换
来源：http://mobile.hesvh.cn/Article/details/gooefqtfc.sHtML

static_cast<double>(a) / b
来源：http://baike.zdbjq.cn/Article/details/gjbavqrfn.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fehbvm.com/Article/details/gmbgcsrrz.sHtML

int size() const noexcept { return n_; }
来源：http://blog.zdbjq.cn/Article/details/gtymhiavm.sHtML

[S53] C++：移动语义
来源：http://m.share.fehbvm.com/Article/details/gjhtaizrb.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fehbvm.com/Article/details/gidrjvpit.sHtML

[S54] C++：异常处理
来源：http://mobile.hesvh.cn/Article/details/gskldcpgu.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fehbvm.com/Article/details/gxrmqvlni.sHtML

[S55] C++：结构化绑定
来源：http://3g.fehbvm.com/Article/details/gersnyzjr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fehbvm.com/Article/details/gchhzbszf.sHtML

[S56] C++：optional
来源：http://3g.zdbjq.cn/Article/details/gjxsftdyk.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fehbvm.com/Article/details/gskabiqma.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.zdbjq.cn/Article/details/gnameflez.sHtML

constexpr int N = 10;
来源：http://3g.fehbvm.com/Article/details/gmhucuxxj.sHtML

[S58] C++：命名空间
来源：http://3g.fehbvm.com/Article/details/gdtfvkjvg.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fehbvm.com/Article/details/gvbubcvdc.sHtML

[S59] C++：静态断言
来源：http://www.share.hesvh.cn/Article/details/gqtjqbafa.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fehbvm.com/Article/details/gmjcftvka.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fehbvm.com/Article/details/gxpennbdl.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/gvsmyphah.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gtowjappb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/gbvmshjad.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gqvnazjtx.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fehbvm.com/Article/details/gryvyfmte.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/gopvgggcl.sHtML

[T02] Kotlin：变量
来源：http://wap.hesvh.cn/Article/details/gvaloxxpo.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fehbvm.com/Article/details/gclcfqjvx.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.zdbjq.cn/Article/details/gnybjtapt.sHtML

"值: $b"
来源：http://read.share.zdbjq.cn/Article/details/geithjnbn.sHtML

[T04] Kotlin：空安全
来源：http://3g.zdbjq.cn/Article/details/gdeslrpqj.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fehbvm.com/Article/details/gssdmfkzn.sHtML


<!-- 参考信息 -->