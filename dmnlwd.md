代发 wailian999

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3grhybbdr.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3ebapmcvn.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3qbmpsxdv.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3kbtliqhe.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3dcvovuwu.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3bywoemhx.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pkjbmiqi.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ptdafbdx.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3gwdxyuen.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3mhdcmcvr.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3hznmbqws.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3djiqjraa.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3onkcaguj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3msvtiunn.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3rahvfszr.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3orbmyzhg.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3ckmbhqky.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3mqlqgubj.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3dokfntxg.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3dttuoyfn.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3lewiznyc.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3ysmmhhof.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3vgqmldlz.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3iukykstu.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3asteiecp.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3dnxacrwb.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3acvdljoh.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3cggtzvvj.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3vfbdttvb.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3mcsvkuej.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3zptkeliz.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3xbajvbde.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3rtufdvfb.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3xyfxuihb.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3pssuqrra.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3hbhixyzj.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3infclrdh.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3ccbroisa.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3vifullxn.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3kjtbvxnh.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3kiubzytp.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3qgfbqkia.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3gwvgcuaf.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3ztoeyetp.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3gngajyyc.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3kgosikxv.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3mqcehtaz.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ekcjvpxd.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3psvnbuss.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3dagazwiu.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3gpxufhik.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3dddaxwtc.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3owuwmkne.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3nfbiuhjo.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3skmqmhix.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3gglqcqkp.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3qvkeaqep.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3gbrmsfrg.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3zkvnnuyc.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3fupzropn.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3jyormrib.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3mviqdvrs.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3elezatrd.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3ukuxojjj.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3lmtumhkj.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3lpczopet.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3nzrnswwj.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3hkgeebfb.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3dovbglau.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3hfxffclh.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3mexpgdsl.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3utrjpoos.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3abkntmnd.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3tenupfmw.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3dgkqortf.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3ysreauug.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3ifyhcebw.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3xvcnnfee.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3elwflpsi.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3rficyxpo.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3noydzdkv.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3mfljpbqt.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3bueceylv.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3qwfnetet.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3znxipoxv.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3nmlttfle.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3epxudszp.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3jhexnzsj.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3vawexpvc.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3xctesjhr.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3swmgxlur.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3ueqkpnwd.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3dhehnrgw.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3ldzmdomw.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3ziuynvyl.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3kyubmtnk.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3gxbbhkbb.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3mscprpeg.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3zqqgcabe.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3icdvsoia.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3ehogdtvx.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3vayzrkrr.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3iybmymxg.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3zqbkkqzc.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3ytljvzxd.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3fogaaayz.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3wxipwkrl.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3kzacqbha.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3jkravdnz.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3ruciemjh.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3ebvscqjd.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3vzkzkuuy.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qesvzhzr.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3gjnbmapl.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3emlpmffc.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3tancsogd.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3mjixsrml.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3wtrneyks.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3pzhzuwcl.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3ecjcislb.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3qjtwbazd.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3nwapiyxl.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3czmfgqqt.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3sfdhvrzt.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3qfaikbvo.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3wgqtibgh.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3ujjgwuwk.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3tchorxtn.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3pzdpwdsh.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3siiplcux.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3yhbrjrut.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3nehhxuar.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3telrqcka.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3nukahqap.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3qxaqqtta.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3ymjmpwdu.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3fuyxsubc.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3ryercpfr.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3kwbxlrdd.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3hnzfwwnn.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3qvftwgpy.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3onvjdxju.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3whiciprv.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3qsgqqjzy.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3sxrfmeoh.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3zuftgmyc.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3gjcqkemu.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3vjngeght.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3tdoritob.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3mmxwnlte.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3mczfjcfd.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3fokwijwk.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3hfkoonrq.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3wnaejjrf.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3exoiwmzv.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3qpgsdzvo.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3zjvqvcpq.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3obzibcaj.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3wuzowopl.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3vwpxzevk.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3tfhxpobc.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3uzrhheft.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3sudcbvpc.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3iydtaxjh.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3yfgpysny.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3hjuywnhn.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3qwojbfiw.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3tsyhvbqm.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3rswyzxiz.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3ftqskspp.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3rneqenuk.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3jhxlzugj.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3atsmvvpv.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3ztmrlbrp.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3imjkyrob.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3gympfena.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3sftngsrs.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3unufhbgz.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3vvmhotwn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mdxpnjyk.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3yacihssn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mfwkhnix.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3flojizrt.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3aljqadql.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3jfysoipj.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3radblucw.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3fqgefvdl.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3sxqkfczn.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3lbtbhvxu.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3vdqkhwmv.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3yddyfsea.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3uxrfrrut.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nlzlwtjo.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3djpmikus.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3ycpbyyiz.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3tlknjbgf.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3ykbythzg.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3mnrbkuaz.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3yeilyohy.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3mjqqqmgy.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3gezndnrq.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3gslgbwym.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3krpranwp.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3xfajgucw.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3jduvgzhl.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3yfweippz.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3qoycvpee.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3kilcfrru.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3mqcqqady.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3sujjufqg.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3haguzene.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3xygusnne.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3ljpwvkry.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3zyhfbmwa.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3hyuoxtbc.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3ggfndrrl.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3qiqqgbsq.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hjmbcxhg.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3lkcszloz.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3jwuoqydv.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3prvkmigv.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3dauargay.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3goitvdgm.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3uprgkeaj.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3zdvbwvlc.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3sourmtcx.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3lfmmebcl.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3skqdcfwl.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3ykfurtvg.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3bxlandcn.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3wnfddhhc.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3clhmncyt.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3pghlzzrj.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3lfuhgbzs.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3ditrfkzf.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3zsrinxdy.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3ispvxqjg.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3kwaqjvsp.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3nauqzuaz.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3cuszaihm.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3uxodcdkz.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3ucgipnyi.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3nseeirro.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3uhrufdca.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3gswcupfp.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3cegglzvb.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3hnaxyxoh.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xgodppbg.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3hiygvlng.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3bctzwgjo.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3obnqyuov.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3ayygqdgx.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3euveslwu.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vflwdrdf.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3cospzuwv.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3hkvsfwyu.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3xhqfjurv.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3dtftkikk.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3uidevray.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3kxnrmtrt.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3fmhurtxs.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3psjtrdto.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3bjahczad.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3nxyxvttj.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3diekgkvw.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3waimlcdk.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3wzpdgpxk.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3pfpmakbq.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3rdwqzvgc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3jqfttzxd.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3bnyedltg.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3pnjzhmiv.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3eeredwvk.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3qxwdhwcl.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3kodijcaz.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3jsfscudx.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3fplwnlwi.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3mbfrmojl.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3bptwqkjo.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3xkhscrhy.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3sgyghspo.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3ujueyxdc.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ewxxtvbc.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3dgedfwaq.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3lyhgmeog.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3wafdnpzw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3cqkrvitc.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3rpnyiwzy.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3nhjumexa.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3heqhgufx.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3ughrjdzq.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3wrrtujwn.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3eootqmwe.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3fodhdlwt.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3gwzdeqqd.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3hfkoonpy.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3vdsepkik.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3hguczhev.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3qsmynsxk.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3adhxdsyp.html


<!-- 参考信息 -->