代发 wailian999

readonly PI=3.14
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggxnmzsse.sHtML

[R04] 位置参数
来源：http://wap.fanxiaobao.xyz/Article/details/gktvlrxgs.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fanxiaobao.xyz/Article/details/grvcapsgp.sHtML

[R05] 参数默认值
来源：http://wap.fanxiaobao.xyz/Article/details/gkhsvcfts.sHtML

name="${1:-default}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gqozwhrnj.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gpeewcepu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavudxbld.sHtML

[R07] if 判断文件
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwuzkmdg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gvavbxhbs.sHtML

[R08] 数值比较
来源：http://blog.fanxiaobao.xyz/Article/details/gbjzfazlc.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gaetmpmvb.sHtML

[R09] 字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gswojzfkk.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfwzdrlka.sHtML

[R10] 正则匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtelvmuq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gbyxcevjr.sHtML

[R11] case 多分支
来源：http://read.share.fanxiaobao.xyz/Article/details/gtmuwechn.sHtML

case "$1" in
来源：http://3g.fanxiaobao.xyz/Article/details/gqxjudftw.sHtML

start) echo "启动" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gztorekry.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzkugmllm.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/grvorsdgx.sHtML

esac
来源：http://blog.fanxiaobao.xyz/Article/details/ghrjwyrcs.sHtML

[R12] for 遍历文件
来源：http://wap.fanxiaobao.xyz/Article/details/gzscryuol.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gglhvvmyj.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gadnvaeza.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/grdvihnct.sHtML

[R14] C 风格 for
来源：http://m.share.fanxiaobao.xyz/Article/details/gkfyxflie.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gsxhblgbl.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbwcsgono.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gzltlfspl.sHtML

[R16] until 等待条件
来源：http://blog.fanxiaobao.xyz/Article/details/gbdapsffi.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/ggvbdvhrc.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmrvspps.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gfzgvrbws.sHtML

[R18] 遍历数组
来源：http://blog.fanxiaobao.xyz/Article/details/gwkhfwvna.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gnodqfwuj.sHtML

[R19] 数组长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gwnwxkrvo.sHtML

echo "${#arr[@]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gpufnqobd.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fanxiaobao.xyz/Article/details/gemddbwek.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gixxkclkr.sHtML

[R21] 字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/ggcxrpopq.sHtML

echo "${#s}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gulasuwpr.sHtML

[R22] 截取子串
来源：http://www.share.fanxiaobao.xyz/Article/details/gpsvgvjrb.sHtML

echo "${s:0:5}"
来源：http://3g.fanxiaobao.xyz/Article/details/gphllpbsn.sHtML

[R23] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzlqmxewn.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fanxiaobao.xyz/Article/details/gceqetxqo.sHtML

[R24] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gxelgirgj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gginqruhl.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fanxiaobao.xyz/Article/details/gtjeigvrq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gvqmxpzeo.sHtML

[R26] 命令替换
来源：http://wap.fanxiaobao.xyz/Article/details/gjfregage.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fanxiaobao.xyz/Article/details/gwrbpfqcy.sHtML

[R27] 算术展开
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxtabxwd.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fanxiaobao.xyz/Article/details/gwkknwnqu.sHtML

[R28] 浮点运算
来源：http://3g.fanxiaobao.xyz/Article/details/gbkuoieql.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fanxiaobao.xyz/Article/details/gyquokvcy.sHtML

[R29] 定义函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gygjjvesc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gdfiuvizp.sHtML

[R30] 函数返回状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gbpaqyjnk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fanxiaobao.xyz/Article/details/geijvzfpv.sHtML

[R31] 局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gipsdurhr.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fanxiaobao.xyz/Article/details/getgkohnt.sHtML

[R32] 参数个数校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxvigsmi.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gieouykvq.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fanxiaobao.xyz/Article/details/guagwztfg.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fanxiaobao.xyz/Article/details/gyfbxffxh.sHtML

[R34] 退出时清理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdewtinkd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gbhghnpwr.sHtML

[R35] 后台执行并等待
来源：http://3g.fanxiaobao.xyz/Article/details/goiiqcxrv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtongsfaj.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmlwmdne.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fanxiaobao.xyz/Article/details/gmgdctsbf.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/glsjfwcap.sHtML

files=$(ls -1)
来源：http://wap.fanxiaobao.xyz/Article/details/gvjenchnz.sHtML

[R38] 管道串联
来源：http://wap.fanxiaobao.xyz/Article/details/ggvpgkzeu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggfkulehn.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gojyvydiv.sHtML

cmd > out.log 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gkcbujwax.sHtML

[R40] 追加写日志
来源：http://wap.fanxiaobao.xyz/Article/details/gkzobkast.sHtML

echo "log" >> out.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gsxqluwtp.sHtML

[R41] 丢弃输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gmwokgseg.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/glnovmvbn.sHtML

[R42] 输入重定向
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guziwvyrf.sHtML

wc -l < a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gcjulpacp.sHtML

[R43] 按名字查找文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gicrdlwfg.sHtML

find . -name "*.log" -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gmmayvlxk.sHtML

[R44] 按修改时间查找
来源：http://3g.fanxiaobao.xyz/Article/details/gnzjslukr.sHtML

find . -mtime -7 -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gjkqnzumf.sHtML

[R45] 批量删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxvsidii.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fanxiaobao.xyz/Article/details/gpljozqzc.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdlvmmisi.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fanxiaobao.xyz/Article/details/gvhfagxdo.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmhmznjjd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gpvkyhxmj.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/ghnbzgmzg.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/grusuglnz.sHtML

[R49] awk 带条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gkaynjqzx.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fanxiaobao.xyz/Article/details/geecdxrlq.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxmtcryh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/ggyvwrjvs.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohdrwtjx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fanxiaobao.xyz/Article/details/gdomcjhaq.sHtML

[R52] 统计行数
来源：http://3g.fanxiaobao.xyz/Article/details/gwthhnrup.sHtML

wc -l a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmnsszrk.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaizkkvmk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gdyanotbd.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gjqleunqq.sHtML

diff a.txt b.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gonfdaexs.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/gfmbfmkzf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxcgotub.sHtML

[R56] 远程拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gixyginir.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/gdxpsiuce.sHtML

[R57] 远程执行命令
来源：http://wap.fanxiaobao.xyz/Article/details/gxkcvnicj.sHtML

ssh user@host 'uptime'
来源：http://wap.fanxiaobao.xyz/Article/details/gxzmijouc.sHtML

[R58] 下载文件
来源：http://blog.fanxiaobao.xyz/Article/details/gzsqizcrc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fanxiaobao.xyz/Article/details/ggusnhxkb.sHtML

[R59] 发 POST JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gouqsfoqw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/gvnnalebj.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gojivobwq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fanxiaobao.xyz/Article/details/getvqtjdi.sHtML

[R61] 磁盘占用
来源：http://wap.fanxiaobao.xyz/Article/details/gnmmiomua.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/gfbujenqm.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fanxiaobao.xyz/Article/details/goyavuvxj.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fanxiaobao.xyz/Article/details/gjyejrcye.sHtML

[R63] 内存与进程
来源：http://blog.fanxiaobao.xyz/Article/details/gvjixrlvd.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fanxiaobao.xyz/Article/details/glfbzkplv.sHtML

[R64] 结束进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqluluetf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fanxiaobao.xyz/Article/details/gywfuahbi.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gykmwfbqt.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fanxiaobao.xyz/Article/details/guxnngwib.sHtML

[R66] 定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gwtfkxrtd.sHtML

crontab -e;  crontab -l
来源：http://mobile.fanxiaobao.xyz/Article/details/ghphraggi.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glfvmyqxk.sHtML

openssl rand -hex 16
来源：http://wap.fanxiaobao.xyz/Article/details/gcoqihbdc.sHtML

[R68] 计算文件校验值
来源：http://mobile.fanxiaobao.xyz/Article/details/grhhjfxic.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gwpryfdsf.sHtML

[R69] 生成随机密码
来源：http://baike.fanxiaobao.xyz/Article/details/gwlieaeal.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fanxiaobao.xyz/Article/details/gpitquqwo.sHtML

[R70] 时间戳与互转
来源：http://baike.fanxiaobao.xyz/Article/details/gtyrubvfd.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpubuswgm.sHtML

[R71] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gvecjviti.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fanxiaobao.xyz/Article/details/gerpiwvna.sHtML

[R72] 等待端口就绪
来源：http://www.share.fanxiaobao.xyz/Article/details/gkgkvbcms.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmuudwrz.sHtML

[R73] 分割大日志
来源：http://3g.fanxiaobao.xyz/Article/details/gduucqyuw.sHtML

split -l 1000 big.log part_
来源：http://wap.fanxiaobao.xyz/Article/details/gfunnqjjd.sHtML

[R74] 批量重命名
来源：http://www.share.fanxiaobao.xyz/Article/details/gflatsiky.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fanxiaobao.xyz/Article/details/geueeqjku.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/ghowmjugf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fanxiaobao.xyz/Article/details/gfjcfypcx.sHtML

[R76] 使用临时文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gktryfcwv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gutydacjs.sHtML

[R77] 读取用户输入
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmocwycq.sHtML

read -rp "请输入: " ans
来源：http://3g.fanxiaobao.xyz/Article/details/gcjoidgmt.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/gypwuzkoj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjvwwofm.sHtML

[R79] 解析命令行选项
来源：http://mobile.fanxiaobao.xyz/Article/details/gkpaidsns.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fanxiaobao.xyz/Article/details/gwnklhjxl.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhwxkpdq.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/gywppqeyi.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejxkehoa.sHtML

S. C / C++ 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gdcmygqfk.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/geyrxakfo.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqnzrdjol.sHtML

#include <stdio.h>
来源：http://mobile.fanxiaobao.xyz/Article/details/gdcypxsfp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fanxiaobao.xyz/Article/details/gtpprxrsd.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geudohsxo.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fanxiaobao.xyz/Article/details/gvikqfhho.sHtML

[S03] C：读入整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxwjpwgx.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fanxiaobao.xyz/Article/details/grqwaxzmr.sHtML

[S04] C：字符串复制
来源：http://blog.fanxiaobao.xyz/Article/details/gdcezezly.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fanxiaobao.xyz/Article/details/ghnrzlcpj.sHtML

[S05] C：字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gvluecjku.sHtML

strlen(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpclfcgp.sHtML

[S06] C：字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gilqsqjdi.sHtML

strcmp(a, b) == 0
来源：http://www.share.fanxiaobao.xyz/Article/details/gbsbipgnn.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gfwhdppcl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fanxiaobao.xyz/Article/details/gukacxnpo.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fanxiaobao.xyz/Article/details/ggjaryylo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdlqeebsv.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fanxiaobao.xyz/Article/details/gtcdklfix.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fanxiaobao.xyz/Article/details/gwedzyvja.sHtML

[S10] C：指针与解引用
来源：http://mobile.fanxiaobao.xyz/Article/details/gfmvyejfo.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fanxiaobao.xyz/Article/details/gjkmefhao.sHtML

[S11] C：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gqsblioeu.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/goziowsbd.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gxcqwkmfl.sHtML

fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjetdjixt.sHtML

[S12] C：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gcxoojbka.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdywdynrd.sHtML

[S13] C：宏定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdpkpwtmc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fanxiaobao.xyz/Article/details/gqrqmrrpt.sHtML

[S14] C：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/guabfaqdt.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fanxiaobao.xyz/Article/details/geaetqrxt.sHtML

[S15] C：类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkyymxbew.sHtML

(double) a / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhbwcqti.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsehisvss.sHtML

x |= (1 << 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gkdhjvodc.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guuprrnov.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzzwzqyqx.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gujgboeat.sHtML

int main(int argc, char **argv)
来源：http://3g.fanxiaobao.xyz/Article/details/gskvuckfj.sHtML

[S19] C：快速排序
来源：http://3g.fanxiaobao.xyz/Article/details/gdeudlzvv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gdhicpphd.sHtML

[S20] C：二分查找
来源：http://mobile.fanxiaobao.xyz/Article/details/ggfevkocu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxpqmwmth.sHtML

[S21] C：字符类别判断
来源：http://www.share.fanxiaobao.xyz/Article/details/gikgkiuto.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/gcbsaazfz.sHtML

[S22] C：字符串转数字
来源：http://3g.fanxiaobao.xyz/Article/details/gjnayomeo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/gtvihqcuf.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/gwbztqxuw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fanxiaobao.xyz/Article/details/goyfdeqhq.sHtML

[S24] C：获取本地时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gaaybvwjt.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fanxiaobao.xyz/Article/details/gbszuqegj.sHtML

[S25] C：内存拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gzestxsci.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggljfzseg.sHtML

[S26] C：内存清零
来源：http://baike.fanxiaobao.xyz/Article/details/geqkeiizz.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fanxiaobao.xyz/Article/details/grihqtkxy.sHtML

[S27] C：定义常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grrguuxta.sHtML

const double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gphirdoaj.sHtML

[S28] C：静态变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqvgcswc.sHtML

static int counter = 0;
来源：http://baike.fanxiaobao.xyz/Article/details/gwesrpmkh.sHtML

[S29] C：变参函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtryieujm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fanxiaobao.xyz/Article/details/gctgfmpyz.sHtML

[S30] C：头文件保护
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmxcgqhsd.sHtML

#ifndef X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gnbtfwjsj.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gxnlhtwsq.sHtML

#endif
来源：http://mobile.fanxiaobao.xyz/Article/details/gygzgunib.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/grlmnoovy.sHtML

#include <iostream>
来源：http://blog.fanxiaobao.xyz/Article/details/gfgdzqurs.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqyeppquz.sHtML

[S32] C++：字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gahpdiyef.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fanxiaobao.xyz/Article/details/gafsuqjpj.sHtML

[S33] C++：vector 增删
来源：http://baike.fanxiaobao.xyz/Article/details/gzcineddy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fanxiaobao.xyz/Article/details/goilemgkn.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fanxiaobao.xyz/Article/details/gyazwfmow.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gfvlrwkmq.sHtML

[S35] C++：map
来源：http://m.share.fanxiaobao.xyz/Article/details/gndlipltr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggplxtzps.sHtML

[S36] C++：unordered_map
来源：http://read.share.fanxiaobao.xyz/Article/details/gnqgtpekd.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gdjmijudn.sHtML

[S37] C++：set
来源：http://mobile.fanxiaobao.xyz/Article/details/goxfutcmo.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnewtgbdo.sHtML

[S38] C++：排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/grpxshpci.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gmtmpbhbr.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/ghvmagdov.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyeqmteak.sHtML

[S40] C++：查找元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gnovfxphc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvgzedfjg.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fanxiaobao.xyz/Article/details/goksexull.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fanxiaobao.xyz/Article/details/glsyuqgwu.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfdzzilfj.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fanxiaobao.xyz/Article/details/gqwgfbumi.sHtML

[S43] C++：智能指针
来源：http://m.share.fanxiaobao.xyz/Article/details/glrujggmd.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fanxiaobao.xyz/Article/details/gxdlbtqhy.sHtML

[S44] C++：引用传参
来源：http://3g.fanxiaobao.xyz/Article/details/ghnqxkznm.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjneohkti.sHtML

[S45] C++：lambda
来源：http://baike.fanxiaobao.xyz/Article/details/gzygqodtg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fanxiaobao.xyz/Article/details/gicaunevi.sHtML

[S46] C++：函数模板
来源：http://3g.fanxiaobao.xyz/Article/details/gibfxflnl.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gjxvcuror.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gbahmrmbr.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvahbijcz.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxtilxypl.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fanxiaobao.xyz/Article/details/gmlsusbgf.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhfchcoe.sHtML

[S49] C++：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gujbsbffr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbtztudnj.sHtML

[S50] C++：格式化数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gjyvjzrih.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvcbverko.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gcipclfaj.sHtML

static_cast<double>(a) / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gefrplcbh.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fanxiaobao.xyz/Article/details/gqqatdecx.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghydsdxdf.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzspppbcg.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fanxiaobao.xyz/Article/details/giocoocrt.sHtML

[S54] C++：异常处理
来源：http://read.share.fanxiaobao.xyz/Article/details/galggzhgn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gclgbrrim.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvgrukpt.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fanxiaobao.xyz/Article/details/grptxqxaz.sHtML

[S56] C++：optional
来源：http://3g.fanxiaobao.xyz/Article/details/ggjqczzdr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gauvdnsxs.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwixmetqz.sHtML

constexpr int N = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gexykwfqe.sHtML

[S58] C++：命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/gtyhauyps.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fanxiaobao.xyz/Article/details/gjnysjenr.sHtML

[S59] C++：静态断言
来源：http://read.share.fanxiaobao.xyz/Article/details/gcaftuwoj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fanxiaobao.xyz/Article/details/gkchwxdnj.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fanxiaobao.xyz/Article/details/gedorggch.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfnfbqvrr.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/grawlbmbu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fanxiaobao.xyz/Article/details/gcppidgzs.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/ggcdabedm.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gegmtkahb.sHtML

println("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/guknwrtah.sHtML

[T02] Kotlin：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gayxmnvpy.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fanxiaobao.xyz/Article/details/gfaivutip.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fanxiaobao.xyz/Article/details/ghnhpjull.sHtML

"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gmbqvbrpj.sHtML

[T04] Kotlin：空安全
来源：http://blog.fanxiaobao.xyz/Article/details/gefpvutba.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fanxiaobao.xyz/Article/details/gfembflhf.sHtML


<!-- 参考信息 -->