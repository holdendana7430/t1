代发 wailian999

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3ugfruzun.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3dpdabyuo.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3trxezuwl.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3tmdthnnh.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3nihgvgzr.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3pfdzkyas.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3xzwjrlwf.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3admflzmn.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3sqxrshfg.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3yahvzwkf.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3llptzrji.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3yziplsea.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3skmmzanv.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3zugelihu.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3rkcqjths.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3yxfkbrty.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3tvodypmk.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3gmsjgjkw.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3narerczv.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3uadymfwh.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3tpkjasbz.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3zymqqyix.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3wxagyzyx.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3lctnrlee.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3fuuotjwh.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3jguswtsf.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3zbxgjddp.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3nlcbphxq.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3foriwnyq.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3fdthgpxw.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3izimiiht.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3jvdtkurk.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3fcrdopac.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3vgcmttne.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3dwqfujai.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3vwljsshu.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3lsextuho.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3rrsezixt.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3bvkppigo.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3ekgyjwrj.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3ljicecur.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3xcqzzrgo.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3omppecbe.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3jcumzpvo.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3onaymvka.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3vxejhzoa.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3ffdscuhd.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3xdbrbvum.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3ndzzioyc.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3jjqtthah.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3reqdmsou.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3bbsuamrk.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3goahgjsu.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3idkuenzy.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3iswagoyv.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3spmzkhiq.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3crjjeotl.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3fhpfkqxt.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3zqcrsjfr.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3kqinaaql.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3gtcdvlvy.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3ngknhzwm.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3oqjwiquf.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3hyhopsui.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3ecwpnybc.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3wbmzsyqk.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3cezqhugc.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3mbrfkdgs.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3ntcvorac.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3zictlixw.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3jrbrecfq.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3btllpfni.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3tbkghgfc.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3tenfnigh.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3yivmibuh.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3awakgrrr.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3tdbuujkn.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3wbtloutv.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3wmrdgqft.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3gvcujftb.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3nrzwehxv.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3qveehrzu.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3zvmafmvk.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3qanjbfpp.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3sdfilbfc.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3dgokzvhp.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wtjfsrug.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3cqhfkxtb.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3ecbphdzi.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3laqrkqyw.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3cjbpiovg.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3awdkucza.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3ujwquyxr.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3ycsdukbg.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3gtsmobxi.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3jbuqqciu.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3sqdiocmq.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3kszyyzxk.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zkrocmbz.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3tjniuoqn.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3rouonffi.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3ovhfnbju.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tdmbfvgw.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3ccrdudzj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3iqbmemwc.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3tnhejnfi.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3chnovxoa.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3laijacwl.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3jranhyfb.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3mfvyrwtn.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gtufzkyy.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3lzmepmbj.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3scjccogv.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3xzlzqvqu.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3gkahefph.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3jqybqtra.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3jzckvytr.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3ywuhdwhi.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3panzckfd.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3fjipksid.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3laxknqqa.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3wrzcwygu.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3lsytesih.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3qpcsxwte.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3dtyyunbo.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3emiekgmd.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3afqtersy.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3xdonrjlm.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3njpuebqs.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3aliywxtj.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3qpnvynrr.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3pcljeypc.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3bssxptnt.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3ynveugwa.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3ljkeljwp.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3cxczbsqy.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3hffircdq.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3wkuthryc.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3nywaexlj.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3phenbmcz.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3aqdrlfrp.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3jyrrsqwm.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3mopzseup.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3wbonsxbw.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3lsivoaew.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3cqixsmyr.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3tzobgxdr.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3lbibxmpa.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3gtlivmym.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3rozjgrgm.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3emznpjni.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3riinytzz.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3xeqgxuzl.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3qwtujpaj.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3fywtxrun.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3bhynheke.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3amottuti.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3awrsolly.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3hpkzaxjd.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3cmaxdgbi.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3udzavluu.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3uhtfzmrm.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3xcaujzcm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dmnvlnlh.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3mikvxpqd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fuxvidal.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dzlmkuzf.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3bqhopkyl.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3huqowbvw.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3kajbpzuv.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3ykccsujr.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3dztzzvfi.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3ulumusug.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3jdoyhdft.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3sxdxpwto.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ozjdqppu.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kyutdxzb.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ijmwcwnp.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3ieeklrkn.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3igltikab.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3fxpswyiw.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3xmlikboo.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3yhyqtcgg.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3dgjhrrxo.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3evqdkukm.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3cvxkxfmk.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3wrltwask.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3idktykan.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3wmphwjph.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3lbvftzim.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3vhrjknfj.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3jeeqfkdb.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ftcmkvsu.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3dpeapxjv.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3ngrxloob.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3sgmtapqz.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3iqhcbuhm.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3yjpxdjhx.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3tpkspxle.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3dseseevm.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3rnempuec.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pbxfrveq.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3ayigepdw.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3myzcimfq.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3dhfopyvf.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3idspmcof.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3wkhqaoid.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3mthunnyp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ujsqwmwq.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3kkitcwux.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3olvassij.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3lucneeyq.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3kajhixya.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3usaahtoc.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3kewmqjgu.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3nbrxrnkq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3xljurutk.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3vlobfhwf.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3hlxubusk.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3lxnouyvm.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3rjtkxpvc.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3ckfzfkxd.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3belwyqqh.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3akkbdynp.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3cxosapgr.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3bakpupas.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3ptwelmyn.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3fhqnmezh.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3eqecuqdu.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3khzcgpcp.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3kgbdwrve.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3fkrkprvj.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3oiffxydq.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3gfqwwpdn.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3ofessddi.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3mhdbwmnm.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3erifjxzg.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ytntmvdp.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3zkqdskpk.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3swpwxgrx.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3xkjieozv.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3holijrao.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3gblxbmrn.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3gttziztb.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3drxbpqsx.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3nzkzljto.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3ruzrbonc.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3xctryuro.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3vddhojvm.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3ebmmmjwl.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3ceeihyss.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gnonotbt.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3dkltvyoe.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3lgptzxlw.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3xxyxizqa.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3obsmtidm.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3wwzxthem.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3yipgyzef.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3icsqvbfd.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3zyntmxct.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3efksztlo.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3qzlhhfag.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3asetfais.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3hzvkabdr.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hzadxaqh.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3cnjyaufr.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3edsimcqi.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3gnvijjqs.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ihpliiig.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3sjgbvdlg.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3mauzyklt.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3eoxpqdhr.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3uqdymvwm.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3jezxeplp.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3vzcsfybf.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3anvkbdfn.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3fkcqxqvz.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3hkzifoct.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3xnwyjbvm.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3tfqhdber.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3sdzjmflw.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3fgvkmrly.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3gplbeyzp.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3cqpxjxko.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3dktqsvrr.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3dvqqhlzq.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3efhlmqsf.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3egboujtp.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3lhldhzyq.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3rdxtdfor.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3jkkyrkww.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3zqstadcc.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3pxdgbwfs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zmmknpzt.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3nvbsaxte.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yjmbxwug.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3durjimqg.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3nidjoryl.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3dxcuvfnu.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3kdqkbgls.html


<!-- 参考信息 -->