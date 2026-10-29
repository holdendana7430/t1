代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://blog.hesvh.cn/Article/details/gyfrcxtcv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.hesvh.cn/Article/details/gluknlotk.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.hesvh.cn/Article/details/guosdkxlq.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fehbvm.com/Article/details/gbdncbaki.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.hesvh.cn/Article/details/gbsxwjepx.sHtML

[Q90] 生成序号列
来源：http://wap.fehbvm.com/Article/details/gfopyadcf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.zdbjq.cn/Article/details/glomfakxm.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/grdldidaz.sHtML

R. Bash 专题
来源：http://www.share.zdbjq.cn/Article/details/gmqtsfdnk.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gihetxpfs.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.hesvh.cn/Article/details/gqmkkojpo.sHtML

#!/usr/bin/env bash
来源：http://www.share.hesvh.cn/Article/details/gojmqeyrq.sHtML

set -euo pipefail
来源：http://www.share.hesvh.cn/Article/details/gdsidxhxb.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fehbvm.com/Article/details/gcngpbcjk.sHtML

name="Tom"; echo "$name"
来源：http://wap.hesvh.cn/Article/details/gmgtngweu.sHtML

[R03] 只读变量
来源：http://wap.fehbvm.com/Article/details/gljakhtxo.sHtML

readonly PI=3.14
来源：http://www.m.share.fehbvm.com/Article/details/guffsfybt.sHtML

[R04] 位置参数
来源：http://m.share.fehbvm.com/Article/details/goqhbtuht.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.hesvh.cn/Article/details/gnsfnzibw.sHtML

[R05] 参数默认值
来源：http://www.m.share.hesvh.cn/Article/details/gtwtuzfqn.sHtML

name="${1:-default}"
来源：http://blog.zdbjq.cn/Article/details/gxktjchdk.sHtML

[R06] 判断命令是否存在
来源：http://3g.fehbvm.com/Article/details/gcbcumlhy.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/gdixhtnku.sHtML

[R07] if 判断文件
来源：http://www.m.share.zdbjq.cn/Article/details/gvpunspdn.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.hesvh.cn/Article/details/gsndiywet.sHtML

[R08] 数值比较
来源：http://wap.zdbjq.cn/Article/details/gbuskgqcw.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.hesvh.cn/Article/details/gyidivkkg.sHtML

[R09] 字符串比较
来源：http://www.share.hesvh.cn/Article/details/gjwlwbmrd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.zdbjq.cn/Article/details/gsayxhumk.sHtML

[R10] 正则匹配
来源：http://www.share.fehbvm.com/Article/details/gwjoyjhtm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.zdbjq.cn/Article/details/gyhibylpp.sHtML

[R11] case 多分支
来源：http://blog.hesvh.cn/Article/details/ggwtrejzv.sHtML

case "$1" in
来源：http://3g.zdbjq.cn/Article/details/grrcegizd.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gfsdvtmzn.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gngralqit.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.zdbjq.cn/Article/details/ghvkbmbmc.sHtML

esac
来源：http://blog.fehbvm.com/Article/details/gfsmvasst.sHtML

[R12] for 遍历文件
来源：http://read.share.zdbjq.cn/Article/details/gldmwbcso.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fehbvm.com/Article/details/gqxvpthat.sHtML

[R13] for 计数循环
来源：http://mobile.fehbvm.com/Article/details/goqxobroo.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/gemxdcgfx.sHtML

[R14] C 风格 for
来源：http://mobile.hesvh.cn/Article/details/gzjpdclmh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gmauvocop.sHtML

[R15] while 逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gekwdmkaw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.zdbjq.cn/Article/details/gwnhgongi.sHtML

[R16] until 等待条件
来源：http://www.m.share.fehbvm.com/Article/details/gcmydmamc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/gpqaqovwj.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fehbvm.com/Article/details/gvutlwbsx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fehbvm.com/Article/details/gmwbpngcf.sHtML

[R18] 遍历数组
来源：http://read.share.fehbvm.com/Article/details/gfdaqbqil.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fehbvm.com/Article/details/gumcyiqeu.sHtML

[R19] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/gkvsvqzqt.sHtML

echo "${#arr[@]}"
来源：http://blog.zdbjq.cn/Article/details/gsneseoit.sHtML

[R20] 关联数组（字典）
来源：http://www.share.zdbjq.cn/Article/details/ghmbzseqk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.hesvh.cn/Article/details/gtsloeffb.sHtML

[R21] 字符串长度
来源：http://m.share.fehbvm.com/Article/details/gfzouqcpl.sHtML

echo "${#s}"
来源：http://wap.fehbvm.com/Article/details/grxwgshju.sHtML

[R22] 截取子串
来源：http://baike.hesvh.cn/Article/details/gjaogvguo.sHtML

echo "${s:0:5}"
来源：http://www.share.hesvh.cn/Article/details/gpcopypsq.sHtML

[R23] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gxpgpnivg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.hesvh.cn/Article/details/gsmbtthpw.sHtML

[R24] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/glqgjxelt.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.hesvh.cn/Article/details/genosbkax.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.hesvh.cn/Article/details/gckvmllvg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.zdbjq.cn/Article/details/gjwlxkirp.sHtML

[R26] 命令替换
来源：http://wap.zdbjq.cn/Article/details/gtmoznlrm.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.hesvh.cn/Article/details/gztczxmgd.sHtML

[R27] 算术展开
来源：http://m.share.fehbvm.com/Article/details/gvivytska.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fehbvm.com/Article/details/grfjewyiq.sHtML

[R28] 浮点运算
来源：http://3g.fehbvm.com/Article/details/gsivwkpit.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.zdbjq.cn/Article/details/gygbzoouw.sHtML

[R29] 定义函数
来源：http://3g.zdbjq.cn/Article/details/goqbrdsvn.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fehbvm.com/Article/details/gtcbjnmkj.sHtML

[R30] 函数返回状态码
来源：http://m.share.fehbvm.com/Article/details/gpbvnghmt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fehbvm.com/Article/details/gcvltqxrn.sHtML

[R31] 局部变量
来源：http://www.share.fehbvm.com/Article/details/gxguftfou.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fehbvm.com/Article/details/gznoppinz.sHtML

[R32] 参数个数校验
来源：http://www.share.fehbvm.com/Article/details/gpkndxsse.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/gbrllxhtp.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.hesvh.cn/Article/details/gmyzaibfb.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.hesvh.cn/Article/details/guibdxlxy.sHtML

[R34] 退出时清理
来源：http://m.share.fehbvm.com/Article/details/gbphlcmjz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/goujyeexq.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fehbvm.com/Article/details/gldduxlhc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fehbvm.com/Article/details/gpwawftph.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.zdbjq.cn/Article/details/gzwrxwpqu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fehbvm.com/Article/details/gnkoghtzs.sHtML

[R37] 把输出赋给变量
来源：http://baike.fehbvm.com/Article/details/glknzbnnx.sHtML

files=$(ls -1)
来源：http://mobile.zdbjq.cn/Article/details/ghokpldrq.sHtML

[R38] 管道串联
来源：http://3g.zdbjq.cn/Article/details/gsarqpbtx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.hesvh.cn/Article/details/gphsvaudt.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.hesvh.cn/Article/details/ginpizcas.sHtML

cmd > out.log 2>&1
来源：http://blog.hesvh.cn/Article/details/glxstyqfa.sHtML

[R40] 追加写日志
来源：http://www.m.share.zdbjq.cn/Article/details/gssznucii.sHtML

echo "log" >> out.log
来源：http://read.share.fehbvm.com/Article/details/gwgxtrawk.sHtML

[R41] 丢弃输出
来源：http://www.blog.hesvh.cn/Article/details/goiyudmli.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fehbvm.com/Article/details/gikrupzyd.sHtML

[R42] 输入重定向
来源：http://m.share.zdbjq.cn/Article/details/gifuyopkj.sHtML

wc -l < a.txt
来源：http://3g.hesvh.cn/Article/details/gydtzoipj.sHtML

[R43] 按名字查找文件
来源：http://3g.zdbjq.cn/Article/details/gkkfwvbbc.sHtML

find . -name "*.log" -type f
来源：http://read.share.zdbjq.cn/Article/details/gkvcypunm.sHtML

[R44] 按修改时间查找
来源：http://wap.hesvh.cn/Article/details/gjmlpoldi.sHtML

find . -mtime -7 -type f
来源：http://mobile.hesvh.cn/Article/details/gsdmvcdfn.sHtML

[R45] 批量删除
来源：http://mobile.hesvh.cn/Article/details/gfdkjwqup.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.hesvh.cn/Article/details/ggxjugfxj.sHtML

[R46] 递归替换文件内容
来源：http://www.share.hesvh.cn/Article/details/garfingvd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.hesvh.cn/Article/details/gzclyqwio.sHtML

[R47] sed 单行替换
来源：http://www.blog.hesvh.cn/Article/details/gwxdzcvjn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fehbvm.com/Article/details/gpvbensud.sHtML

[R48] awk 取指定列
来源：http://mobile.fehbvm.com/Article/details/gsixxjtnb.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fehbvm.com/Article/details/ghkfwqerd.sHtML

[R49] awk 带条件
来源：http://read.share.fehbvm.com/Article/details/gpckijwmt.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.zdbjq.cn/Article/details/gvecyfmko.sHtML

[R50] awk 求和
来源：http://mobile.fehbvm.com/Article/details/gggfprfjk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/ghvddcarr.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.hesvh.cn/Article/details/gmvmxsxvw.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.zdbjq.cn/Article/details/gpaotjnes.sHtML

[R52] 统计行数
来源：http://m.share.zdbjq.cn/Article/details/gqkwnhwin.sHtML

wc -l a.txt
来源：http://baike.fehbvm.com/Article/details/grdtsosov.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.zdbjq.cn/Article/details/gxhwqwujz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.hesvh.cn/Article/details/gzvsidpnm.sHtML

[R54] 比较两个文件
来源：http://m.share.zdbjq.cn/Article/details/gpqidwyaq.sHtML

diff a.txt b.txt
来源：http://3g.hesvh.cn/Article/details/gswxxxtvm.sHtML

[R55] 压缩与解压
来源：http://www.m.share.hesvh.cn/Article/details/grenmqtve.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.zdbjq.cn/Article/details/gblgtqvls.sHtML

[R56] 远程拷贝
来源：http://mobile.fehbvm.com/Article/details/gvowixodo.sHtML

scp file user@host:/path/
来源：http://www.blog.fehbvm.com/Article/details/gyjacyazj.sHtML

[R57] 远程执行命令
来源：http://3g.hesvh.cn/Article/details/gdurpntol.sHtML

ssh user@host 'uptime'
来源：http://baike.fehbvm.com/Article/details/ghmrnntok.sHtML

[R58] 下载文件
来源：http://mobile.hesvh.cn/Article/details/gowyoehnx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fehbvm.com/Article/details/gjoholvac.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fehbvm.com/Article/details/gqojrszcn.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.zdbjq.cn/Article/details/gadfwoxby.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/gramhvkbr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.zdbjq.cn/Article/details/gcmqpvxab.sHtML

[R61] 磁盘占用
来源：http://www.share.zdbjq.cn/Article/details/gstvwkqjd.sHtML

df -h;  du -sh *
来源：http://m.share.fehbvm.com/Article/details/gaqagvwdh.sHtML

[R62] 找最占空间的文件
来源：http://wap.zdbjq.cn/Article/details/gtdtasbgs.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.hesvh.cn/Article/details/gpojymgjk.sHtML

[R63] 内存与进程
来源：http://3g.hesvh.cn/Article/details/gvedfnull.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.hesvh.cn/Article/details/gspujayyu.sHtML

[R64] 结束进程
来源：http://www.share.fehbvm.com/Article/details/gftcojwbo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.zdbjq.cn/Article/details/gsxdavwew.sHtML

[R65] 查看端口占用
来源：http://m.share.hesvh.cn/Article/details/gpypifhux.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fehbvm.com/Article/details/gpqlpjldw.sHtML

[R66] 定时任务
来源：http://blog.zdbjq.cn/Article/details/gbbblxqvd.sHtML

crontab -e;  crontab -l
来源：http://www.share.fehbvm.com/Article/details/gfchmdfof.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.hesvh.cn/Article/details/grkdszvsz.sHtML

openssl rand -hex 16
来源：http://www.blog.fehbvm.com/Article/details/goejcbllt.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fehbvm.com/Article/details/ghhosewbm.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.zdbjq.cn/Article/details/gcwhkwmuo.sHtML

[R69] 生成随机密码
来源：http://m.share.hesvh.cn/Article/details/gxjuabwjj.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.hesvh.cn/Article/details/gjobumvtf.sHtML

[R70] 时间戳与互转
来源：http://wap.hesvh.cn/Article/details/gcrhnniyi.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fehbvm.com/Article/details/gapesgokf.sHtML

[R71] 日期格式化
来源：http://wap.fehbvm.com/Article/details/gbokfonxp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.zdbjq.cn/Article/details/gilacyqdn.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fehbvm.com/Article/details/gzepmwhca.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/gvmjbwmac.sHtML

[R73] 分割大日志
来源：http://3g.fehbvm.com/Article/details/gmjmjxvqg.sHtML

split -l 1000 big.log part_
来源：http://3g.fehbvm.com/Article/details/gwuynoeig.sHtML

[R74] 批量重命名
来源：http://mobile.zdbjq.cn/Article/details/gtebeprqa.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fehbvm.com/Article/details/gdvdeabct.sHtML

[R75] 导出环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gmsymomnd.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.zdbjq.cn/Article/details/gxqesvurx.sHtML

[R76] 使用临时文件
来源：http://3g.zdbjq.cn/Article/details/gpzflatqq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/gxjpqiqaa.sHtML

[R77] 读取用户输入
来源：http://www.blog.zdbjq.cn/Article/details/gmctollsi.sHtML

read -rp "请输入: " ans
来源：http://mobile.zdbjq.cn/Article/details/gdnofvxzy.sHtML

[R78] 交互式菜单
来源：http://www.m.share.zdbjq.cn/Article/details/glxfpxuhm.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.hesvh.cn/Article/details/gpmdmfbfp.sHtML

[R79] 解析命令行选项
来源：http://3g.zdbjq.cn/Article/details/gpnfxdvqs.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.hesvh.cn/Article/details/gkhkafogl.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.zdbjq.cn/Article/details/gbeghogws.sHtML

time ./run.sh
来源：http://wap.fehbvm.com/Article/details/grpzldtxb.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gwwltjpif.sHtML

S. C / C++ 专题
来源：http://mobile.hesvh.cn/Article/details/glrfrwwxn.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gvjttdsgn.sHtML

[S01] C：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gioldusar.sHtML

#include <stdio.h>
来源：http://www.blog.fehbvm.com/Article/details/gvidyiqjp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.hesvh.cn/Article/details/ggjnwyfrn.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.hesvh.cn/Article/details/gbqupbgmv.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fehbvm.com/Article/details/gzynkdeaa.sHtML

[S03] C：读入整数
来源：http://mobile.fehbvm.com/Article/details/gebuiqaib.sHtML

int x; scanf("%d", &x);
来源：http://blog.zdbjq.cn/Article/details/gmblnhjhn.sHtML

[S04] C：字符串复制
来源：http://baike.hesvh.cn/Article/details/gdcojgfyh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.zdbjq.cn/Article/details/gtoxljavm.sHtML

[S05] C：字符串长度
来源：http://read.share.hesvh.cn/Article/details/gmhtqoowm.sHtML

strlen(s)
来源：http://m.share.zdbjq.cn/Article/details/gfrokrqts.sHtML

[S06] C：字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gdlwfddgv.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fehbvm.com/Article/details/grpqnkfgj.sHtML

[S07] C：数组遍历求和
来源：http://www.share.hesvh.cn/Article/details/gxubcbxol.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.hesvh.cn/Article/details/gqbjiehig.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fehbvm.com/Article/details/grmhadjee.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fehbvm.com/Article/details/grdkbzvrm.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.zdbjq.cn/Article/details/gcdwtrisj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fehbvm.com/Article/details/gafkgtjtl.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fehbvm.com/Article/details/gynzzegmc.sHtML

int *p = &a;  *p = 5;
来源：http://blog.hesvh.cn/Article/details/gawwdznws.sHtML

[S11] C：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/ghnhyvxhr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.zdbjq.cn/Article/details/grvtpxcyl.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fehbvm.com/Article/details/gaarwhatd.sHtML

fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gmjvqajwv.sHtML

[S12] C：写文件
来源：http://www.blog.fehbvm.com/Article/details/grplvdgqt.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/gjvhiseeq.sHtML

[S13] C：宏定义
来源：http://mobile.zdbjq.cn/Article/details/gngexjoej.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.zdbjq.cn/Article/details/ghqjdgmye.sHtML

[S14] C：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/genztdvdn.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.hesvh.cn/Article/details/glugcnrpr.sHtML

[S15] C：类型转换
来源：http://www.share.fehbvm.com/Article/details/gfwvhmkzr.sHtML

(double) a / b
来源：http://wap.fehbvm.com/Article/details/gkpuecclr.sHtML

[S16] C：位操作置位
来源：http://blog.fehbvm.com/Article/details/gexodaedj.sHtML

x |= (1 << 3);
来源：http://blog.zdbjq.cn/Article/details/gqqslknhv.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gdpvrgdnh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fehbvm.com/Article/details/gsbnppfqz.sHtML

[S18] C：命令行参数
来源：http://blog.zdbjq.cn/Article/details/gbsqikiuu.sHtML

int main(int argc, char **argv)
来源：http://mobile.fehbvm.com/Article/details/ghrgngvmy.sHtML

[S19] C：快速排序
来源：http://mobile.fehbvm.com/Article/details/gyqxrhlaz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/gmspsixmo.sHtML

[S20] C：二分查找
来源：http://www.share.zdbjq.cn/Article/details/gbhotrbwp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/genoaigyc.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fehbvm.com/Article/details/grkdaxbtb.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.hesvh.cn/Article/details/gtlbpzpbr.sHtML

[S22] C：字符串转数字
来源：http://blog.zdbjq.cn/Article/details/gmnnhdadr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fehbvm.com/Article/details/gcwfwhbtx.sHtML

[S23] C：随机数
来源：http://read.share.hesvh.cn/Article/details/gtpafrcuo.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fehbvm.com/Article/details/glkmdkjbx.sHtML

[S24] C：获取本地时间
来源：http://www.blog.zdbjq.cn/Article/details/gdsslqwiy.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.zdbjq.cn/Article/details/gwzvywdpb.sHtML

[S25] C：内存拷贝
来源：http://baike.zdbjq.cn/Article/details/guhsndfod.sHtML

memcpy(dst, src, n);
来源：http://wap.fehbvm.com/Article/details/gkricqjpk.sHtML

[S26] C：内存清零
来源：http://m.share.hesvh.cn/Article/details/gkscosczd.sHtML

memset(a, 0, sizeof a);
来源：http://wap.zdbjq.cn/Article/details/gxukcvxmn.sHtML

[S27] C：定义常量
来源：http://blog.fehbvm.com/Article/details/gzigonhnf.sHtML

const double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gscysngta.sHtML

[S28] C：静态变量
来源：http://3g.hesvh.cn/Article/details/gxdjcolbp.sHtML

static int counter = 0;
来源：http://m.share.zdbjq.cn/Article/details/gmmpsnjcj.sHtML

[S29] C：变参函数
来源：http://www.blog.zdbjq.cn/Article/details/gqmbggvzp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fehbvm.com/Article/details/gzzrzpzkr.sHtML

[S30] C：头文件保护
来源：http://baike.fehbvm.com/Article/details/gxozgjduc.sHtML

#ifndef X_H
来源：http://wap.zdbjq.cn/Article/details/gywruvbom.sHtML

#define X_H
来源：http://wap.fehbvm.com/Article/details/gagdcncqr.sHtML

#endif
来源：http://blog.zdbjq.cn/Article/details/gqumumrof.sHtML

[S31] C++：Hello World
来源：http://blog.zdbjq.cn/Article/details/gnpehpbxl.sHtML

#include <iostream>
来源：http://www.blog.hesvh.cn/Article/details/gudyaxgot.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.zdbjq.cn/Article/details/geraoqnpa.sHtML

[S32] C++：字符串
来源：http://www.m.share.hesvh.cn/Article/details/gkvetdvmh.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fehbvm.com/Article/details/gvhkibyxq.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.zdbjq.cn/Article/details/gzyvzoymr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fehbvm.com/Article/details/gssdmtofs.sHtML

[S34] C++：遍历 vector
来源：http://mobile.hesvh.cn/Article/details/goocrhvhl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.zdbjq.cn/Article/details/gjwpbizzn.sHtML

[S35] C++：map
来源：http://wap.fehbvm.com/Article/details/gdchzblpy.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gvnbfebgo.sHtML

[S36] C++：unordered_map
来源：http://3g.hesvh.cn/Article/details/gzyghcprc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/ghrdlculx.sHtML

[S37] C++：set
来源：http://read.share.hesvh.cn/Article/details/gdsrywvjk.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fehbvm.com/Article/details/glmpwbxex.sHtML

[S38] C++：排序
来源：http://blog.fehbvm.com/Article/details/gbqbkcuth.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.zdbjq.cn/Article/details/gzfuedsde.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.hesvh.cn/Article/details/gscgfltnw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.zdbjq.cn/Article/details/gnrqubllq.sHtML

[S40] C++：查找元素
来源：http://mobile.hesvh.cn/Article/details/gywvbgfov.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fehbvm.com/Article/details/ghedioqiz.sHtML

[S41] C++：类与构造函数
来源：http://3g.hesvh.cn/Article/details/gfujxggqv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.hesvh.cn/Article/details/gakjpcgli.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.zdbjq.cn/Article/details/gwbojkbyg.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.hesvh.cn/Article/details/gvjetnuzr.sHtML

[S43] C++：智能指针
来源：http://blog.fehbvm.com/Article/details/giznsmlpo.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fehbvm.com/Article/details/gecgntuyz.sHtML

[S44] C++：引用传参
来源：http://3g.zdbjq.cn/Article/details/gtxspxqgu.sHtML

void inc(int &x) { ++x; }
来源：http://3g.hesvh.cn/Article/details/gjijdquvg.sHtML

[S45] C++：lambda
来源：http://www.m.share.fehbvm.com/Article/details/glsuqpvnn.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fehbvm.com/Article/details/gwziusulp.sHtML

[S46] C++：函数模板
来源：http://m.share.hesvh.cn/Article/details/ghdkkjlyb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fehbvm.com/Article/details/gdxatpifx.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fehbvm.com/Article/details/gnearplje.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fehbvm.com/Article/details/gtqpwbhei.sHtML

[S48] C++：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/geudlwqbr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.hesvh.cn/Article/details/ggvibzeqs.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.hesvh.cn/Article/details/gjrlwgwew.sHtML

[S49] C++：写文件
来源：http://read.share.zdbjq.cn/Article/details/ghgzqqcru.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.zdbjq.cn/Article/details/guwbmzgbd.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fehbvm.com/Article/details/gmwemnict.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gtwgyqgyl.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gjpkcrveo.sHtML

static_cast<double>(a) / b
来源：http://www.blog.zdbjq.cn/Article/details/gbsydfret.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fehbvm.com/Article/details/gwwpqvyqy.sHtML

int size() const noexcept { return n_; }
来源：http://wap.hesvh.cn/Article/details/gnllaeyov.sHtML

[S53] C++：移动语义
来源：http://m.share.fehbvm.com/Article/details/gxpldfavy.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.zdbjq.cn/Article/details/gyobhtwfd.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fehbvm.com/Article/details/gduszkgxs.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.zdbjq.cn/Article/details/gkvaqubdn.sHtML

[S55] C++：结构化绑定
来源：http://3g.hesvh.cn/Article/details/grpyngqdk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.hesvh.cn/Article/details/gskgytiwd.sHtML

[S56] C++：optional
来源：http://mobile.zdbjq.cn/Article/details/gpyxssqtx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.zdbjq.cn/Article/details/gfezdgsst.sHtML

[S57] C++：编译期常量
来源：http://wap.hesvh.cn/Article/details/gtiiwprmq.sHtML

constexpr int N = 10;
来源：http://baike.fehbvm.com/Article/details/gvmhmntkt.sHtML

[S58] C++：命名空间
来源：http://mobile.hesvh.cn/Article/details/gfsyvhxdv.sHtML


<!-- 参考信息 -->