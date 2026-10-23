代发 wailian999

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3mqyprwqf.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bonyglxp.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3rpqczdjz.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3ypjnczfp.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3eorfwgaj.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3cqoskgkg.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3nhcdhysi.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3izthyraw.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3ubntthpf.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3gukpuvqw.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3unkfkynu.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3snwlebzi.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3fvctonzg.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3mhqrbnqm.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3orphwekx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vtthqzxk.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3eejnbpul.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tpsqsbsm.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3wtvoxbhr.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3zeowbtxi.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3uflihxkv.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3fbbzcbpf.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3wipnoslu.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3xeurgrqz.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3ipxpiilm.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3gtlmznnr.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3ednwvnbp.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3idfcmbdt.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3smluyhqt.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3lzlgfiwt.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3qzepdvge.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3ccvnbbyz.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3pulofaow.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3kudeuhqj.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3kgmrcepu.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3dqpcbnoj.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3dxdrtsjf.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3xtnaffmp.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3iivjqlwx.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3uhdqtdor.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3vpqkiocl.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3lmosiqdd.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3fxbevnmb.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3twvwjtuu.html

esac
来源：http://www.52xcode.cn/Article/details/gt3uzgyctlg.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3gnuzhmwa.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3qveuezln.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3yscrcvvr.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3atjmlldw.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3ognxayru.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3vmsjvbti.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3tsznkszi.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qjpawnoz.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3jeiynapx.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3glblsynr.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3peegyvuu.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3uncvavtk.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3ymaakffj.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3zipjucki.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3nokedent.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3hyjsntvx.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3mvbwhkyz.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3ndktonas.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3dwvfctbk.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3cgltmlwp.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3vdyeijee.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3imdxynof.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3qrhaglfr.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3wvwuqang.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3xzblphqg.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3adsrxrvm.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3xpyzcrbb.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3uzmlwigp.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3vqtgtjlh.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3lnkhpqii.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3niyoijrt.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3xzvppwmk.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3mofosfni.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3lbhimoya.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3dtcnyqox.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3bmeyrxai.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3rlsvggsa.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3xxyzoifm.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3naduexhh.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3avpdefsj.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3kymtsibr.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3eactlleh.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3nugannve.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3geabnpvu.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3ooemotut.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3uhejkmzp.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3aizlowjp.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3rbnvqhhl.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3uznkgrzx.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3wswsvmfn.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3zwvqmxmv.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3ccigynss.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3fghwdtfb.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3pvxpgkev.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3pmklxulu.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3lpqvdjpk.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3rcmoszpy.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3xobqwhib.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3uvifqswc.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3oqtbikik.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3mpwianwb.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3pmzgjiol.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3xkypvjnv.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3pvdkfwap.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3bsbsotjy.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3gqyznqtt.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3rzfvrmpg.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3iyldgfgc.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3adguleqi.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3bjrdtqfh.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3skdpflrw.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wjxymljc.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3bukgclsw.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3zzdjrzyn.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3lgkaivje.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3gqqlbkon.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3rrhimhzv.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3hocjgvnf.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3kjfgukhv.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3siwtalei.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3hcsosfub.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3eossqved.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3gvwrteod.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3cbkockwl.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3bjegkfqb.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3plkewacf.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3cwtyvawq.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3xqufloet.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ksrgurll.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3zytqjkxw.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3mjrpqbpc.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3vtjubnkf.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3nforqqfa.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3gltdmsmz.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3jzstvnqh.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3nnhzwgqt.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3vmnqqqyv.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3aqasgwvc.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3epsjpzmu.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3jpytulyc.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3aoltabdn.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3dzyycljs.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3ibnpaxgh.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3kiaptzix.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3opyalmsu.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3vibtlfqu.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3vfhgjwze.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3kehquvmj.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3srmpxzvb.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3pwauuayx.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3usynwfcd.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3ccrfylxb.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3ebbrtcxz.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3oyrbhoor.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3yuivwbbj.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3gcztdeju.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3tdclxyof.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3fbzrzqnk.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3mkmcrxqn.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3nuqwukxt.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3rxrqmbgi.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3pwtdlutu.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3retthrbt.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3umayxsdp.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3dinjcfdm.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3quqjnbks.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ogbalbky.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3fqynzufe.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3unwmtdce.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3lntdvepl.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3ruttatmr.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3arvjtoul.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3pxgxfbjs.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3twqonbnn.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3rdowyeko.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3exfnguln.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3phiviaeh.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3vuqgfmam.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jivduzlw.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3ceznqjtz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3unhigcur.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ikimmped.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3rrwlakbw.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3ghlxymxt.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3covjtlyo.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3rbkizzty.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3rzotggpq.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3bqpttwbp.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3gipeqods.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3gwjpdjjp.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3bmiklniv.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3uihudogi.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3igkfkxpn.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3uovnstcz.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3vrlqimcd.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3kyhoqrws.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3ctibbtsj.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3fnpohhzz.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3boicgmmq.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3kgmqargl.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3zdgsuyxg.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3nhsdloiq.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ayhduspv.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3ymldxiaf.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3qgslbheq.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3qzwuowyq.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3jzcxhyyf.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3mzjbpzls.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3bwawlhyp.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3bentewni.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3spaztvfw.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3ylhvgdvf.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3mvuaqpxx.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3pwuxhhyt.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3peeewrzu.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jorlzpfk.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3lcrbhmbd.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3zweajnlg.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3iasdjbnk.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3iezxbqza.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3xcpyjxcm.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3rthveqnl.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3szsruhwm.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3nyvqquae.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3qfycqbml.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3jnhodsje.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3uqlmzcuu.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3tkhqqeoj.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3oxqshiox.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3zfvzatqj.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3wlzevuge.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3qggkodst.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3tyncixrz.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3nzdjajoq.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3vgubwxsn.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3bszahwik.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3kngnhors.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3dkrvutiz.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3msadnqdn.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3kwtfsdlt.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3ewixhxzx.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3ehplutbj.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3uonnwgbk.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3ydppjtwe.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3bezrspdy.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3srvheedk.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3olhwxxcc.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3ghhokkfp.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3kjkbyuqg.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3crqoycpb.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3qtxvhvak.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3podjfrnn.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kozusyou.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3ycidwnrp.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3retkrokd.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3ludgrkcj.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3gwmuiqmc.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3nwzozlzs.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3doooqcpk.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3vgljdbij.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3cbdjbxcs.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3ezkekfzu.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3biucvzaw.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3ytvscnxp.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3mnwctzdo.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3cpjuqnvn.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3vuwfrvse.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3kordcfno.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3xamjnydh.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3fnorkmrk.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3gbvzcptp.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3kzkuvajs.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3lnswhmag.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3yikqrnva.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3eikirsci.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3vxqmfcvh.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3vncshooj.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3jrabhiwg.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3pyevkmse.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3zsnlgukd.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3bfdlbryf.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3uawlxaio.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3chsbkndd.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3xterzfbm.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3imnihnnv.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3szsvqbrk.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3yzyhkkmx.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3qwhhrbjc.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3ogwualoa.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3vydaqjhq.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3futwedig.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3menmjvkp.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3jvzqienf.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3jrjxdbnz.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3irvbuugi.html


<!-- 参考信息 -->