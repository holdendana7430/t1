代发 wailian999

set -euo pipefail
来源：http://www.blog.hesvh.cn/Article/details/gcsngudxd.sHtML

[R02] 变量赋值与使用
来源：http://mobile.zdbjq.cn/Article/details/gbstklywi.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fehbvm.com/Article/details/ggqbvdnvz.sHtML

[R03] 只读变量
来源：http://www.share.fehbvm.com/Article/details/gjcpbwfmf.sHtML

readonly PI=3.14
来源：http://read.share.fehbvm.com/Article/details/gqfkofspt.sHtML

[R04] 位置参数
来源：http://www.blog.fehbvm.com/Article/details/gspwncxja.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.zdbjq.cn/Article/details/giwvjnpty.sHtML

[R05] 参数默认值
来源：http://blog.hesvh.cn/Article/details/gnhserhow.sHtML

name="${1:-default}"
来源：http://read.share.hesvh.cn/Article/details/gpbsdnybc.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fehbvm.com/Article/details/giacanlxl.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gavslxhjk.sHtML

[R07] if 判断文件
来源：http://baike.zdbjq.cn/Article/details/gzzxstaji.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gufioggzl.sHtML

[R08] 数值比较
来源：http://www.m.share.hesvh.cn/Article/details/gjsioasca.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.hesvh.cn/Article/details/gnsezcoli.sHtML

[R09] 字符串比较
来源：http://www.share.fehbvm.com/Article/details/gcbxlbtoy.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.hesvh.cn/Article/details/gmmjojdmt.sHtML

[R10] 正则匹配
来源：http://www.share.zdbjq.cn/Article/details/gwioqbjgy.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.hesvh.cn/Article/details/glvgaryiz.sHtML

[R11] case 多分支
来源：http://baike.fehbvm.com/Article/details/gqczthqbf.sHtML

case "$1" in
来源：http://mobile.hesvh.cn/Article/details/gitbcyiru.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fehbvm.com/Article/details/geicjmejy.sHtML

stop)  echo "停止" ;;
来源：http://blog.hesvh.cn/Article/details/ggxnapecg.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.hesvh.cn/Article/details/glbvuusho.sHtML

esac
来源：http://baike.hesvh.cn/Article/details/gnpqqcdax.sHtML

[R12] for 遍历文件
来源：http://baike.zdbjq.cn/Article/details/gofirpzzv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fehbvm.com/Article/details/gkhkhcomc.sHtML

[R13] for 计数循环
来源：http://www.share.fehbvm.com/Article/details/gegiknekw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/gwvsbfsbt.sHtML

[R14] C 风格 for
来源：http://blog.hesvh.cn/Article/details/gjxmugkvz.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/guoketxic.sHtML

[R15] while 逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gfnatezyx.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fehbvm.com/Article/details/gvtlayqxz.sHtML

[R16] until 等待条件
来源：http://m.share.zdbjq.cn/Article/details/gavipikek.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/gbrwfpfoq.sHtML

[R17] 数组定义与取值
来源：http://read.share.zdbjq.cn/Article/details/gsjksjdpp.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.hesvh.cn/Article/details/gfpinzhxv.sHtML

[R18] 遍历数组
来源：http://www.m.share.hesvh.cn/Article/details/gltlfhxft.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.hesvh.cn/Article/details/gvtglanmv.sHtML

[R19] 数组长度
来源：http://wap.fehbvm.com/Article/details/ggpxohzqj.sHtML

echo "${#arr[@]}"
来源：http://m.share.hesvh.cn/Article/details/gyumsvtkr.sHtML

[R20] 关联数组（字典）
来源：http://baike.zdbjq.cn/Article/details/gxhlazmxq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fehbvm.com/Article/details/gytxexrup.sHtML

[R21] 字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gcqssnlox.sHtML

echo "${#s}"
来源：http://www.m.share.hesvh.cn/Article/details/gcgiibzds.sHtML

[R22] 截取子串
来源：http://3g.hesvh.cn/Article/details/goiqakfkv.sHtML

echo "${s:0:5}"
来源：http://wap.hesvh.cn/Article/details/gvkqeulgp.sHtML

[R23] 字符串替换
来源：http://wap.fehbvm.com/Article/details/gyljxnjwz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.zdbjq.cn/Article/details/grdkqgwej.sHtML

[R24] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gvzxtdslp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.zdbjq.cn/Article/details/gcfhgjumg.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fehbvm.com/Article/details/gupzngugq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fehbvm.com/Article/details/gvjkrfkyc.sHtML

[R26] 命令替换
来源：http://blog.fehbvm.com/Article/details/geyikxnfd.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fehbvm.com/Article/details/grnizpcgt.sHtML

[R27] 算术展开
来源：http://3g.fehbvm.com/Article/details/gxtvvafxj.sHtML

echo $((1 + 2 * 3))
来源：http://baike.zdbjq.cn/Article/details/gvoudfnyw.sHtML

[R28] 浮点运算
来源：http://www.blog.hesvh.cn/Article/details/gpkqtgohw.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.zdbjq.cn/Article/details/gumadxtzo.sHtML

[R29] 定义函数
来源：http://read.share.zdbjq.cn/Article/details/gnjcaqrzf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.hesvh.cn/Article/details/gwivildaz.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fehbvm.com/Article/details/gjavusspv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.hesvh.cn/Article/details/gcvkybtuw.sHtML

[R31] 局部变量
来源：http://m.share.zdbjq.cn/Article/details/gveogkjiu.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.zdbjq.cn/Article/details/gzfrosvuv.sHtML

[R32] 参数个数校验
来源：http://wap.fehbvm.com/Article/details/gkbldbqle.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/gnbjwfgro.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fehbvm.com/Article/details/gtnxrkyju.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.hesvh.cn/Article/details/gzhagfrde.sHtML

[R34] 退出时清理
来源：http://www.blog.fehbvm.com/Article/details/gyykbzfja.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gseolxgmk.sHtML

[R35] 后台执行并等待
来源：http://3g.hesvh.cn/Article/details/gvbnlqzpf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fehbvm.com/Article/details/gxaslsgyn.sHtML

[R36] 并发执行多个任务
来源：http://www.share.hesvh.cn/Article/details/gjpyuqqrc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.hesvh.cn/Article/details/gyajuuaqz.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fehbvm.com/Article/details/gynlhbksh.sHtML

files=$(ls -1)
来源：http://baike.zdbjq.cn/Article/details/gbzbqoujl.sHtML

[R38] 管道串联
来源：http://baike.fehbvm.com/Article/details/gdbokibon.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fehbvm.com/Article/details/gcvhtmefy.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fehbvm.com/Article/details/gntxsxjdo.sHtML

cmd > out.log 2>&1
来源：http://www.share.hesvh.cn/Article/details/gumvsvjsd.sHtML

[R40] 追加写日志
来源：http://blog.fehbvm.com/Article/details/gzktswcfh.sHtML

echo "log" >> out.log
来源：http://m.share.fehbvm.com/Article/details/gpuwodzwi.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fehbvm.com/Article/details/gspzkpclb.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/gikrsozrl.sHtML

[R42] 输入重定向
来源：http://m.share.fehbvm.com/Article/details/gzxywwyfy.sHtML

wc -l < a.txt
来源：http://read.share.fehbvm.com/Article/details/gabmbqjfe.sHtML

[R43] 按名字查找文件
来源：http://mobile.zdbjq.cn/Article/details/gljwrgfev.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.zdbjq.cn/Article/details/gebhxbuod.sHtML

[R44] 按修改时间查找
来源：http://m.share.zdbjq.cn/Article/details/gqvjojwwh.sHtML

find . -mtime -7 -type f
来源：http://read.share.zdbjq.cn/Article/details/gacgexjnx.sHtML

[R45] 批量删除
来源：http://baike.fehbvm.com/Article/details/gildqgioh.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fehbvm.com/Article/details/gdtssffsy.sHtML

[R46] 递归替换文件内容
来源：http://m.share.zdbjq.cn/Article/details/gccusmlar.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.zdbjq.cn/Article/details/gvfvjzapj.sHtML

[R47] sed 单行替换
来源：http://m.share.hesvh.cn/Article/details/gmpkgwkla.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.hesvh.cn/Article/details/gaulboepa.sHtML

[R48] awk 取指定列
来源：http://read.share.fehbvm.com/Article/details/gpamgueqb.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fehbvm.com/Article/details/gydqgzsyt.sHtML

[R49] awk 带条件
来源：http://www.m.share.fehbvm.com/Article/details/glhycwluw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.hesvh.cn/Article/details/gvkrcxire.sHtML

[R50] awk 求和
来源：http://mobile.hesvh.cn/Article/details/gbzwdswnj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gdppiqobs.sHtML

[R51] 排序去重取前几
来源：http://baike.zdbjq.cn/Article/details/gduwqdcqw.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.hesvh.cn/Article/details/gegjvnhgf.sHtML

[R52] 统计行数
来源：http://read.share.fehbvm.com/Article/details/gbfjrfhsx.sHtML

wc -l a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gxswljfva.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.hesvh.cn/Article/details/gkaognqcb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fehbvm.com/Article/details/ghuyozove.sHtML

[R54] 比较两个文件
来源：http://mobile.fehbvm.com/Article/details/gfjskzihc.sHtML

diff a.txt b.txt
来源：http://www.share.fehbvm.com/Article/details/ghhnyjuoh.sHtML

[R55] 压缩与解压
来源：http://wap.hesvh.cn/Article/details/glvtrmnzf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fehbvm.com/Article/details/gclaulwtf.sHtML

[R56] 远程拷贝
来源：http://3g.fehbvm.com/Article/details/gzxdhdehj.sHtML

scp file user@host:/path/
来源：http://mobile.zdbjq.cn/Article/details/gayfbtfzp.sHtML

[R57] 远程执行命令
来源：http://www.blog.hesvh.cn/Article/details/gungsepje.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.hesvh.cn/Article/details/giluyjogo.sHtML

[R58] 下载文件
来源：http://blog.hesvh.cn/Article/details/gjebxjjnz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.hesvh.cn/Article/details/gkbilweei.sHtML

[R59] 发 POST JSON
来源：http://3g.fehbvm.com/Article/details/glknjnnnf.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.zdbjq.cn/Article/details/gxphfobcl.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/goruoluez.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.zdbjq.cn/Article/details/gbggxafzw.sHtML

[R61] 磁盘占用
来源：http://blog.hesvh.cn/Article/details/gnoiudynf.sHtML

df -h;  du -sh *
来源：http://www.blog.zdbjq.cn/Article/details/gxaedhtle.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fehbvm.com/Article/details/gsuuscglv.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.zdbjq.cn/Article/details/gnnlajsqt.sHtML

[R63] 内存与进程
来源：http://m.share.fehbvm.com/Article/details/glkdrnqpw.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.hesvh.cn/Article/details/gufjszcxc.sHtML

[R64] 结束进程
来源：http://3g.fehbvm.com/Article/details/gflcrwzic.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.zdbjq.cn/Article/details/gelrhkjoz.sHtML

[R65] 查看端口占用
来源：http://read.share.fehbvm.com/Article/details/grbqcvjfh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fehbvm.com/Article/details/goidabrac.sHtML

[R66] 定时任务
来源：http://read.share.zdbjq.cn/Article/details/gcempbhil.sHtML

crontab -e;  crontab -l
来源：http://baike.zdbjq.cn/Article/details/gsmwvomlg.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.zdbjq.cn/Article/details/gthtkkziz.sHtML

openssl rand -hex 16
来源：http://read.share.fehbvm.com/Article/details/gkffednmk.sHtML

[R68] 计算文件校验值
来源：http://www.blog.zdbjq.cn/Article/details/gkcwykfqb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fehbvm.com/Article/details/gvdgfmjlr.sHtML

[R69] 生成随机密码
来源：http://baike.hesvh.cn/Article/details/gwbtneniq.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fehbvm.com/Article/details/guraqvhmt.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fehbvm.com/Article/details/getoanhfl.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.zdbjq.cn/Article/details/gkiqijuad.sHtML

[R71] 日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/guhkprftv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.hesvh.cn/Article/details/gsfeonugx.sHtML

[R72] 等待端口就绪
来源：http://wap.hesvh.cn/Article/details/gwqftmbkg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/garoqsnhj.sHtML

[R73] 分割大日志
来源：http://read.share.hesvh.cn/Article/details/goxfsxdov.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fehbvm.com/Article/details/gpvgguvfv.sHtML

[R74] 批量重命名
来源：http://3g.hesvh.cn/Article/details/gjckltnrr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.hesvh.cn/Article/details/gapgirbdy.sHtML

[R75] 导出环境变量
来源：http://wap.hesvh.cn/Article/details/gptxvfrke.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.hesvh.cn/Article/details/geronyjdn.sHtML

[R76] 使用临时文件
来源：http://3g.zdbjq.cn/Article/details/gpfmymzyt.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/gxgdqvlii.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fehbvm.com/Article/details/gxrsthhhk.sHtML

read -rp "请输入: " ans
来源：http://wap.hesvh.cn/Article/details/gfighpsry.sHtML

[R78] 交互式菜单
来源：http://wap.fehbvm.com/Article/details/gabngwpzt.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fehbvm.com/Article/details/glouilikf.sHtML

[R79] 解析命令行选项
来源：http://3g.fehbvm.com/Article/details/gmqnjtzng.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.hesvh.cn/Article/details/gvyrcayai.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.zdbjq.cn/Article/details/gflpvmbhw.sHtML

time ./run.sh
来源：http://mobile.hesvh.cn/Article/details/gadphnkcd.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gnrknlkla.sHtML

S. C / C++ 专题
来源：http://www.share.fehbvm.com/Article/details/gaoxkrdqi.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/grgvkoums.sHtML

[S01] C：Hello World
来源：http://3g.fehbvm.com/Article/details/gfnkqefdz.sHtML

#include <stdio.h>
来源：http://m.share.fehbvm.com/Article/details/ghqdunaan.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.zdbjq.cn/Article/details/gyjlbwxse.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.hesvh.cn/Article/details/gfqhhyqfn.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.hesvh.cn/Article/details/gucdpgchc.sHtML

[S03] C：读入整数
来源：http://read.share.zdbjq.cn/Article/details/gdshavdjn.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.hesvh.cn/Article/details/grceawwoq.sHtML

[S04] C：字符串复制
来源：http://3g.zdbjq.cn/Article/details/ghwtpnael.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fehbvm.com/Article/details/grwyzeyjr.sHtML

[S05] C：字符串长度
来源：http://www.share.fehbvm.com/Article/details/gprivrczh.sHtML

strlen(s)
来源：http://blog.fehbvm.com/Article/details/gukblqjvx.sHtML

[S06] C：字符串比较
来源：http://3g.hesvh.cn/Article/details/gissawuxm.sHtML

strcmp(a, b) == 0
来源：http://3g.fehbvm.com/Article/details/gfohpsjps.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.zdbjq.cn/Article/details/gkrkeanzz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fehbvm.com/Article/details/gcbfvaurm.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.zdbjq.cn/Article/details/gondzbmeh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.zdbjq.cn/Article/details/gxtlyeaor.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.hesvh.cn/Article/details/gwupemmwd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fehbvm.com/Article/details/gehnhakvn.sHtML

[S10] C：指针与解引用
来源：http://wap.zdbjq.cn/Article/details/gzcjlvicx.sHtML

int *p = &a;  *p = 5;
来源：http://3g.hesvh.cn/Article/details/gbsexrycj.sHtML

[S11] C：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/glxkfgtrb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.zdbjq.cn/Article/details/gnbuvjyel.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fehbvm.com/Article/details/gjwjpiyki.sHtML

fclose(f);
来源：http://blog.zdbjq.cn/Article/details/gassiajkw.sHtML

[S12] C：写文件
来源：http://www.share.zdbjq.cn/Article/details/gbyljgqov.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gjytcpqnx.sHtML

[S13] C：宏定义
来源：http://mobile.zdbjq.cn/Article/details/gkzzajwue.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.zdbjq.cn/Article/details/gncqwbzpa.sHtML

[S14] C：枚举
来源：http://www.blog.zdbjq.cn/Article/details/gjwmijtwn.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.hesvh.cn/Article/details/gfzmnvzqo.sHtML

[S15] C：类型转换
来源：http://m.share.hesvh.cn/Article/details/gqdhxlkaw.sHtML

(double) a / b
来源：http://read.share.zdbjq.cn/Article/details/geokzyzyr.sHtML

[S16] C：位操作置位
来源：http://read.share.hesvh.cn/Article/details/gdtbwwqol.sHtML

x |= (1 << 3);
来源：http://m.share.fehbvm.com/Article/details/gluvaekgm.sHtML

[S17] C：安全拼接字符串
来源：http://wap.zdbjq.cn/Article/details/girgwwvnb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.zdbjq.cn/Article/details/goewtqwiz.sHtML

[S18] C：命令行参数
来源：http://baike.zdbjq.cn/Article/details/gesfwlnbo.sHtML

int main(int argc, char **argv)
来源：http://wap.fehbvm.com/Article/details/guumbgcvn.sHtML

[S19] C：快速排序
来源：http://mobile.fehbvm.com/Article/details/graeuxnxm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gagzxmuqd.sHtML

[S20] C：二分查找
来源：http://blog.hesvh.cn/Article/details/guijqdimf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/gfjudjage.sHtML

[S21] C：字符类别判断
来源：http://www.share.zdbjq.cn/Article/details/gkyktfukt.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.hesvh.cn/Article/details/gtclffokp.sHtML

[S22] C：字符串转数字
来源：http://www.blog.hesvh.cn/Article/details/gvwqyasss.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fehbvm.com/Article/details/gezjlhuvf.sHtML

[S23] C：随机数
来源：http://m.share.fehbvm.com/Article/details/ghdwocfar.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fehbvm.com/Article/details/googfpdko.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fehbvm.com/Article/details/gbgsgdrhl.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.hesvh.cn/Article/details/gwyfyciro.sHtML

[S25] C：内存拷贝
来源：http://baike.fehbvm.com/Article/details/ghhxfjdcp.sHtML

memcpy(dst, src, n);
来源：http://3g.fehbvm.com/Article/details/gabqpskdo.sHtML

[S26] C：内存清零
来源：http://read.share.zdbjq.cn/Article/details/gcwdpxuml.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.zdbjq.cn/Article/details/gzaiggtwn.sHtML

[S27] C：定义常量
来源：http://m.share.zdbjq.cn/Article/details/gpuinuizd.sHtML

const double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gxlgqwjdj.sHtML

[S28] C：静态变量
来源：http://mobile.zdbjq.cn/Article/details/gbtewlgrg.sHtML

static int counter = 0;
来源：http://wap.fehbvm.com/Article/details/gfmogeivh.sHtML

[S29] C：变参函数
来源：http://www.blog.fehbvm.com/Article/details/gqvlxcqfj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.hesvh.cn/Article/details/gbmcsfnik.sHtML

[S30] C：头文件保护
来源：http://m.share.hesvh.cn/Article/details/gdwrdhoyt.sHtML

#ifndef X_H
来源：http://www.share.zdbjq.cn/Article/details/gdshtvagt.sHtML

#define X_H
来源：http://read.share.hesvh.cn/Article/details/gkuzyujel.sHtML

#endif
来源：http://www.share.fehbvm.com/Article/details/gupjwogcd.sHtML

[S31] C++：Hello World
来源：http://www.blog.fehbvm.com/Article/details/guvvscdaw.sHtML

#include <iostream>
来源：http://3g.zdbjq.cn/Article/details/gqjrmxkmm.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmngtvyuz.sHtML

[S32] C++：字符串
来源：http://mobile.zdbjq.cn/Article/details/glfqysepe.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fehbvm.com/Article/details/grqftehbf.sHtML

[S33] C++：vector 增删
来源：http://www.blog.zdbjq.cn/Article/details/ghcmifsam.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.hesvh.cn/Article/details/gfvxolhpn.sHtML

[S34] C++：遍历 vector
来源：http://wap.hesvh.cn/Article/details/gtrhkiftj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fehbvm.com/Article/details/gqygwacrw.sHtML

[S35] C++：map
来源：http://baike.zdbjq.cn/Article/details/gxsvekszr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/grtqvmdnh.sHtML

[S36] C++：unordered_map
来源：http://baike.fehbvm.com/Article/details/gaujlkpwg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gbmufgpwx.sHtML

[S37] C++：set
来源：http://wap.fehbvm.com/Article/details/gqofbbudy.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.hesvh.cn/Article/details/gvlfxhdod.sHtML

[S38] C++：排序
来源：http://3g.hesvh.cn/Article/details/gswepotlp.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.zdbjq.cn/Article/details/gblmjcehs.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.hesvh.cn/Article/details/greqpugez.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fehbvm.com/Article/details/gsvedspjb.sHtML

[S40] C++：查找元素
来源：http://read.share.hesvh.cn/Article/details/glfnfdtle.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.hesvh.cn/Article/details/gxrpqjnlt.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fehbvm.com/Article/details/grsivpxub.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fehbvm.com/Article/details/gbestudpu.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.zdbjq.cn/Article/details/gslvtlwlv.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.hesvh.cn/Article/details/gcyxnbdiu.sHtML

[S43] C++：智能指针
来源：http://mobile.hesvh.cn/Article/details/gbxpedwkn.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.hesvh.cn/Article/details/gmwbeoxoj.sHtML

[S44] C++：引用传参
来源：http://www.share.fehbvm.com/Article/details/gxmkklkcm.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.hesvh.cn/Article/details/ggsnftzpi.sHtML

[S45] C++：lambda
来源：http://www.share.zdbjq.cn/Article/details/gurbbvugi.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.zdbjq.cn/Article/details/gswxmmjwj.sHtML

[S46] C++：函数模板
来源：http://m.share.zdbjq.cn/Article/details/gjrwjcdvm.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fehbvm.com/Article/details/gzwgwsipu.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fehbvm.com/Article/details/gqzindhky.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.hesvh.cn/Article/details/ggkjzoprs.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/ggwmyhveu.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.hesvh.cn/Article/details/gxcynkumm.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gfcqibxif.sHtML

[S49] C++：写文件
来源：http://wap.fehbvm.com/Article/details/gtgxmchjn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fehbvm.com/Article/details/gorvbsqck.sHtML

[S50] C++：格式化数字
来源：http://blog.fehbvm.com/Article/details/gipnlbhbl.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gckridyve.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.hesvh.cn/Article/details/gjrhvhgwn.sHtML

static_cast<double>(a) / b
来源：http://mobile.zdbjq.cn/Article/details/gkflhxewa.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fehbvm.com/Article/details/gawultrld.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fehbvm.com/Article/details/gdobnfwzp.sHtML

[S53] C++：移动语义
来源：http://read.share.hesvh.cn/Article/details/gskmbugtg.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.hesvh.cn/Article/details/gtrcbbocg.sHtML

[S54] C++：异常处理
来源：http://baike.hesvh.cn/Article/details/geawdcqoq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.zdbjq.cn/Article/details/gsminlarn.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fehbvm.com/Article/details/gfhlwflok.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.zdbjq.cn/Article/details/gdmpcaxbl.sHtML

[S56] C++：optional
来源：http://3g.zdbjq.cn/Article/details/gtmcqalqg.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.zdbjq.cn/Article/details/gppzkyfbb.sHtML

[S57] C++：编译期常量
来源：http://baike.zdbjq.cn/Article/details/gkxeznmdw.sHtML

constexpr int N = 10;
来源：http://read.share.zdbjq.cn/Article/details/gmrbkgmry.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fehbvm.com/Article/details/gfccifthc.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.zdbjq.cn/Article/details/glcjpevcg.sHtML

[S59] C++：静态断言
来源：http://m.share.hesvh.cn/Article/details/guwvwxzxh.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.hesvh.cn/Article/details/gonuetukp.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fehbvm.com/Article/details/gfrnohcnb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.zdbjq.cn/Article/details/gpbixxxto.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/giibcviqa.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.zdbjq.cn/Article/details/gxyfzazfk.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gdumwywqv.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gmjzoctkm.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/gyoglyhbl.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.zdbjq.cn/Article/details/gkclavlqm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.zdbjq.cn/Article/details/gonbygjbv.sHtML


<!-- 参考信息 -->