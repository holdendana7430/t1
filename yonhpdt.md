代发 wailian999

[Q84] 去除首尾空格
来源：http://read.share.fanxiaobao.xyz/Article/details/gmxvayprm.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggsicgjpj.sHtML

[Q85] 数值取整
来源：http://www.share.fanxiaobao.xyz/Article/details/gpysmwbfi.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fanxiaobao.xyz/Article/details/gtagglblq.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fanxiaobao.xyz/Article/details/gvnjxyoni.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fanxiaobao.xyz/Article/details/gammqvmte.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gmzmhjkel.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fanxiaobao.xyz/Article/details/govguvpby.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fanxiaobao.xyz/Article/details/gytxtihrb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwxkfuus.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmfktlha.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggycrqeae.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/geakkeidi.sHtML

[Q90] 生成序号列
来源：http://blog.fanxiaobao.xyz/Article/details/gqjchpokx.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggokbnwty.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gpkbupqey.sHtML

R. Bash 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gzdtsiezp.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/grjptaetx.sHtML

[R01] shebang 与严格模式
来源：http://wap.fanxiaobao.xyz/Article/details/gkfsugsfw.sHtML

#!/usr/bin/env bash
来源：http://wap.fanxiaobao.xyz/Article/details/gqjgapiaf.sHtML

set -euo pipefail
来源：http://www.share.fanxiaobao.xyz/Article/details/ggdindirh.sHtML

[R02] 变量赋值与使用
来源：http://3g.fanxiaobao.xyz/Article/details/gsqelqiur.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gncperdmx.sHtML

[R03] 只读变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gegbevrew.sHtML

readonly PI=3.14
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwfmzvqbb.sHtML

[R04] 位置参数
来源：http://read.share.fanxiaobao.xyz/Article/details/guqjguyct.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fanxiaobao.xyz/Article/details/gurrdnblc.sHtML

[R05] 参数默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/gblivhvls.sHtML

name="${1:-default}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gyiiyjhdj.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gfwekmhgw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gipsxwysc.sHtML

[R07] if 判断文件
来源：http://m.share.fanxiaobao.xyz/Article/details/glkfcgbdt.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gtkabzxfh.sHtML

[R08] 数值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/grdjnnaip.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gcvjwutwe.sHtML

[R09] 字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/getnmycdz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gbnepzqzm.sHtML

[R10] 正则匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grftbvzhf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gdhbohmtl.sHtML

[R11] case 多分支
来源：http://blog.fanxiaobao.xyz/Article/details/gttkmvyra.sHtML

case "$1" in
来源：http://m.share.fanxiaobao.xyz/Article/details/glqdbsgjf.sHtML

start) echo "启动" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/grffsqjar.sHtML

stop)  echo "停止" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gpvkwcwbi.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/ghlurlzap.sHtML

esac
来源：http://baike.fanxiaobao.xyz/Article/details/gtajtrlif.sHtML

[R12] for 遍历文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gprqbdblq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gjxsymkcm.sHtML

[R13] for 计数循环
来源：http://3g.fanxiaobao.xyz/Article/details/grfgootvc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gsndlppun.sHtML

[R14] C 风格 for
来源：http://www.share.fanxiaobao.xyz/Article/details/gcwcoxinr.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqrtrtvfq.sHtML

[R15] while 逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gbttlhutz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gtlvbntrs.sHtML

[R16] until 等待条件
来源：http://mobile.fanxiaobao.xyz/Article/details/glvcjcdjd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfaavxakv.sHtML

[R17] 数组定义与取值
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmqqvnar.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gevgvyrdc.sHtML

[R18] 遍历数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/giinmtogo.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gwtexblis.sHtML

[R19] 数组长度
来源：http://baike.fanxiaobao.xyz/Article/details/gqiiryhes.sHtML

echo "${#arr[@]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdgxarik.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fanxiaobao.xyz/Article/details/gslvycpls.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghlygmuxr.sHtML

[R21] 字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gufotpsel.sHtML

echo "${#s}"
来源：http://3g.fanxiaobao.xyz/Article/details/gjifbslhj.sHtML

[R22] 截取子串
来源：http://wap.fanxiaobao.xyz/Article/details/gepuoisev.sHtML

echo "${s:0:5}"
来源：http://baike.fanxiaobao.xyz/Article/details/getuuezxj.sHtML

[R23] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gtipspeun.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fanxiaobao.xyz/Article/details/ggeisgpfh.sHtML

[R24] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxydmfnam.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fanxiaobao.xyz/Article/details/gjcagnvtc.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fanxiaobao.xyz/Article/details/gctpfbgdd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gphioilbb.sHtML

[R26] 命令替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzymikwec.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fanxiaobao.xyz/Article/details/gwzrcexes.sHtML

[R27] 算术展开
来源：http://blog.fanxiaobao.xyz/Article/details/guzvcwwcr.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fanxiaobao.xyz/Article/details/gskfgoafe.sHtML

[R28] 浮点运算
来源：http://www.share.fanxiaobao.xyz/Article/details/gigopijzw.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fanxiaobao.xyz/Article/details/gwyfsllpl.sHtML

[R29] 定义函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwwhbpoo.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/gehncaahl.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gckfhxrmf.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fanxiaobao.xyz/Article/details/gtxtgelyi.sHtML

[R31] 局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gmsjkwbva.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwdkoqgdi.sHtML

[R32] 参数个数校验
来源：http://blog.fanxiaobao.xyz/Article/details/gjaomugon.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glfiwtlaf.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gwpwaodfz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/gskewxwpv.sHtML

[R34] 退出时清理
来源：http://wap.fanxiaobao.xyz/Article/details/gwygxlcqa.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/ggwbbbwkj.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwtynflli.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fanxiaobao.xyz/Article/details/gujfodpmm.sHtML

[R36] 并发执行多个任务
来源：http://blog.fanxiaobao.xyz/Article/details/gkflhyoup.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fanxiaobao.xyz/Article/details/grzecedue.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gthtypdja.sHtML

files=$(ls -1)
来源：http://wap.fanxiaobao.xyz/Article/details/gzqomoron.sHtML

[R38] 管道串联
来源：http://www.share.fanxiaobao.xyz/Article/details/gygehfyiu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fanxiaobao.xyz/Article/details/gquurnnuu.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmwoyymb.sHtML

cmd > out.log 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/geugicvcq.sHtML

[R40] 追加写日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gsnbyzjys.sHtML

echo "log" >> out.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvhapgrr.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/gtlklhflp.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gymerfagu.sHtML

[R42] 输入重定向
来源：http://www.share.fanxiaobao.xyz/Article/details/gbmoiukfk.sHtML

wc -l < a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gbvgbnscf.sHtML

[R43] 按名字查找文件
来源：http://blog.fanxiaobao.xyz/Article/details/gbnsjvfkd.sHtML

find . -name "*.log" -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/galvdmyxz.sHtML

[R44] 按修改时间查找
来源：http://mobile.fanxiaobao.xyz/Article/details/ghlktlcsx.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvksheqhd.sHtML

[R45] 批量删除
来源：http://mobile.fanxiaobao.xyz/Article/details/giiartxpm.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvrwuxcbd.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqygflxpy.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fanxiaobao.xyz/Article/details/gtolycmif.sHtML

[R47] sed 单行替换
来源：http://blog.fanxiaobao.xyz/Article/details/gcsgxbmem.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gyjfitbmz.sHtML

[R48] awk 取指定列
来源：http://baike.fanxiaobao.xyz/Article/details/gnjohwpej.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gvmflpplq.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzkbmfld.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fanxiaobao.xyz/Article/details/guuyrpbez.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwzuzlvbu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gzucxmdvi.sHtML

[R51] 排序去重取前几
来源：http://3g.fanxiaobao.xyz/Article/details/gzrvizous.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gorttdrox.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/gsuaqrung.sHtML

wc -l a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwwrxabj.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fanxiaobao.xyz/Article/details/gjqpxglyb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/grhxgcxxw.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvcwdsuh.sHtML

diff a.txt b.txt
来源：http://wap.fanxiaobao.xyz/Article/details/glstzooqc.sHtML

[R55] 压缩与解压
来源：http://blog.fanxiaobao.xyz/Article/details/gqfbzhsuv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fanxiaobao.xyz/Article/details/grqpqfrgz.sHtML

[R56] 远程拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/godqfxgrd.sHtML

scp file user@host:/path/
来源：http://www.blog.fanxiaobao.xyz/Article/details/gueniaykz.sHtML

[R57] 远程执行命令
来源：http://blog.fanxiaobao.xyz/Article/details/gbylfvhfw.sHtML

ssh user@host 'uptime'
来源：http://baike.fanxiaobao.xyz/Article/details/gnpivswsm.sHtML

[R58] 下载文件
来源：http://blog.fanxiaobao.xyz/Article/details/gmxsekwbj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/ghrfvfamy.sHtML

[R59] 发 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gmxhvvgkd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fanxiaobao.xyz/Article/details/gkvccnynx.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gkzrmpleo.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fanxiaobao.xyz/Article/details/geocjvcrf.sHtML

[R61] 磁盘占用
来源：http://wap.fanxiaobao.xyz/Article/details/gwighwhar.sHtML

df -h;  du -sh *
来源：http://m.share.fanxiaobao.xyz/Article/details/gzgugnner.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gersvoifl.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/gmrfxebxc.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gnaxuwthp.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fanxiaobao.xyz/Article/details/ghmdembcn.sHtML

[R64] 结束进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjsiglrkw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fanxiaobao.xyz/Article/details/gupnyfnca.sHtML

[R65] 查看端口占用
来源：http://blog.fanxiaobao.xyz/Article/details/gmshoflvh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fanxiaobao.xyz/Article/details/gtktwjoyd.sHtML

[R66] 定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gnbfrqtge.sHtML

crontab -e;  crontab -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gxjzayjht.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fanxiaobao.xyz/Article/details/gozjipyjs.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/gjnggzxfs.sHtML

[R68] 计算文件校验值
来源：http://baike.fanxiaobao.xyz/Article/details/giirgpvly.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gvdqyymlv.sHtML

[R69] 生成随机密码
来源：http://baike.fanxiaobao.xyz/Article/details/gikjidsru.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fanxiaobao.xyz/Article/details/gywsihhoj.sHtML

[R70] 时间戳与互转
来源：http://mobile.fanxiaobao.xyz/Article/details/ghxdgrnyv.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fanxiaobao.xyz/Article/details/gfzgzuqet.sHtML

[R71] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gynseosky.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fanxiaobao.xyz/Article/details/gtrauxevh.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/gdmbplexb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gqijikcnv.sHtML

[R73] 分割大日志
来源：http://wap.fanxiaobao.xyz/Article/details/grycsczrq.sHtML

split -l 1000 big.log part_
来源：http://blog.fanxiaobao.xyz/Article/details/gjfoowdjs.sHtML

[R74] 批量重命名
来源：http://www.share.fanxiaobao.xyz/Article/details/ghyijgnbd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gyoqgjvpj.sHtML

[R75] 导出环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gjbdnwtya.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fanxiaobao.xyz/Article/details/gwomhgxhz.sHtML

[R76] 使用临时文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gqegetfoh.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwganxxm.sHtML

[R77] 读取用户输入
来源：http://mobile.fanxiaobao.xyz/Article/details/gcrvbiydy.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggmuubslx.sHtML

[R78] 交互式菜单
来源：http://blog.fanxiaobao.xyz/Article/details/gxqksrriy.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gnggrwjmz.sHtML

[R79] 解析命令行选项
来源：http://m.share.fanxiaobao.xyz/Article/details/gkpazkvqx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fanxiaobao.xyz/Article/details/gwfpyndui.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fanxiaobao.xyz/Article/details/gcjihyjkh.sHtML

time ./run.sh
来源：http://m.share.fanxiaobao.xyz/Article/details/gjalbpkxq.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gevpvcdtn.sHtML

S. C / C++ 专题
来源：http://3g.fanxiaobao.xyz/Article/details/ggirjpbzf.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/godjnbtpg.sHtML

[S01] C：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gtxluvrfh.sHtML

#include <stdio.h>
来源：http://wap.fanxiaobao.xyz/Article/details/gkiamrmnq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gskjrdosn.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gkaysgcvf.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjiduiqq.sHtML

[S03] C：读入整数
来源：http://blog.fanxiaobao.xyz/Article/details/gwkszxcek.sHtML

int x; scanf("%d", &x);
来源：http://baike.fanxiaobao.xyz/Article/details/gzvmxqtvl.sHtML

[S04] C：字符串复制
来源：http://mobile.fanxiaobao.xyz/Article/details/gaaxvjfmd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzvzsehl.sHtML

[S05] C：字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gvaskqwjm.sHtML

strlen(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/guvrjvcnc.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gabsjlnkt.sHtML

strcmp(a, b) == 0
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwtfzfch.sHtML

[S07] C：数组遍历求和
来源：http://wap.fanxiaobao.xyz/Article/details/gsubbjoga.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fanxiaobao.xyz/Article/details/glbftqbts.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyndeelrs.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fanxiaobao.xyz/Article/details/gwhmkeocv.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fanxiaobao.xyz/Article/details/gomxlynla.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fanxiaobao.xyz/Article/details/glmcvyrbn.sHtML

[S10] C：指针与解引用
来源：http://m.share.fanxiaobao.xyz/Article/details/grumcqpin.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fanxiaobao.xyz/Article/details/gkfnwkmyr.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqyxdliq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/gppttsjzj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gdbrlcilf.sHtML

fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/giloeeklx.sHtML

[S12] C：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/givipgcwn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqcxewetd.sHtML

[S13] C：宏定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghkrzksnr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fanxiaobao.xyz/Article/details/gchplujqm.sHtML

[S14] C：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/ggmnfnlqd.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fanxiaobao.xyz/Article/details/gupzumiub.sHtML

[S15] C：类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/giffxtoks.sHtML

(double) a / b
来源：http://wap.fanxiaobao.xyz/Article/details/gwdzwjshq.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghtoqvgfl.sHtML

x |= (1 << 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzrjcjyzv.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gqygvvaza.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcuomeofz.sHtML

[S18] C：命令行参数
来源：http://mobile.fanxiaobao.xyz/Article/details/ggeerhobu.sHtML

int main(int argc, char **argv)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdzriuox.sHtML

[S19] C：快速排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gfrrlfwps.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gywfdmtbg.sHtML

[S20] C：二分查找
来源：http://3g.fanxiaobao.xyz/Article/details/gzdscejuu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqoognpg.sHtML

[S21] C：字符类别判断
来源：http://wap.fanxiaobao.xyz/Article/details/gsjojrztg.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhbswyou.sHtML

[S22] C：字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/geqctsbel.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fanxiaobao.xyz/Article/details/gqwofpvqm.sHtML

[S23] C：随机数
来源：http://www.share.fanxiaobao.xyz/Article/details/gjudxjblq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gwyjmfsmh.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjqksbqc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjnjybgoc.sHtML

[S25] C：内存拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrsmmnbu.sHtML

memcpy(dst, src, n);
来源：http://blog.fanxiaobao.xyz/Article/details/gihnxsrrb.sHtML

[S26] C：内存清零
来源：http://read.share.fanxiaobao.xyz/Article/details/gotvnvnip.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fanxiaobao.xyz/Article/details/gzkmfjqxj.sHtML

[S27] C：定义常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefuhrxnz.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpgrfebps.sHtML

[S28] C：静态变量
来源：http://3g.fanxiaobao.xyz/Article/details/gjyqbdtxm.sHtML

static int counter = 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdaliwpwd.sHtML

[S29] C：变参函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gsptapxhl.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gynpeyqyi.sHtML

[S30] C：头文件保护
来源：http://blog.fanxiaobao.xyz/Article/details/gquzrvujh.sHtML

#ifndef X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gfjldchjs.sHtML

#define X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmcwxuaoz.sHtML

#endif
来源：http://blog.fanxiaobao.xyz/Article/details/gwfdcrckp.sHtML

[S31] C++：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpgaufmgk.sHtML

#include <iostream>
来源：http://3g.fanxiaobao.xyz/Article/details/geslzaqka.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gxcpxqsfs.sHtML

[S32] C++：字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/glhkymbyw.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwynkfrz.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpbbfkyff.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gidtqemli.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fanxiaobao.xyz/Article/details/gvzlyqchu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gxkmfyxqg.sHtML

[S35] C++：map
来源：http://wap.fanxiaobao.xyz/Article/details/gaatjpisr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gutzybfse.sHtML

[S36] C++：unordered_map
来源：http://3g.fanxiaobao.xyz/Article/details/gykortlpk.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaaldrtcz.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/gbuvhvkvy.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ganhrxori.sHtML

[S38] C++：排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmtdyqpsz.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gxhmjlsjr.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/grfbnaoac.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fanxiaobao.xyz/Article/details/gaswimgpo.sHtML

[S40] C++：查找元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gpnpahbfp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyhmwzath.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gkwtvdojs.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnjnfxmuf.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gwonuuoxv.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fanxiaobao.xyz/Article/details/glefijndw.sHtML

[S43] C++：智能指针
来源：http://m.share.fanxiaobao.xyz/Article/details/gikjrqipi.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggwkijkly.sHtML

[S44] C++：引用传参
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfnwhrotd.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmliyotlc.sHtML

[S45] C++：lambda
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdnuuhmom.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gscfmuads.sHtML

[S46] C++：函数模板
来源：http://blog.fanxiaobao.xyz/Article/details/gbmvqlfqq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gqukklybq.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gtaxgjhrn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fanxiaobao.xyz/Article/details/gmvuwlzzp.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtafpsfc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwudwcgnk.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gousgzkqe.sHtML

[S49] C++：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gwwkoursx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/glhfbxfao.sHtML

[S50] C++：格式化数字
来源：http://baike.fanxiaobao.xyz/Article/details/ggopdgszw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkasfwxkr.sHtML

[S51] C++：显式类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gzzxylazd.sHtML

static_cast<double>(a) / b
来源：http://baike.fanxiaobao.xyz/Article/details/gyqtqkhbv.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fanxiaobao.xyz/Article/details/ghlsxeewx.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcgvalbfz.sHtML

[S53] C++：移动语义
来源：http://www.share.fanxiaobao.xyz/Article/details/gohppidvw.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fanxiaobao.xyz/Article/details/gjjjsxtjw.sHtML

[S54] C++：异常处理
来源：http://m.share.fanxiaobao.xyz/Article/details/ggpjgkazo.sHtML


<!-- 参考信息 -->