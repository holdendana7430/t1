代发 wailian999

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2hdtxlioy.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2kouyxzux.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2dbjozahr.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2gvwtibdr.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2neahkxrb.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2hgwzooeh.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2igdoejib.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2ljtfnwls.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2rdrsrcdm.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jvkvqzag.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ptomfvfu.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2krwiaxru.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2nbkptesw.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dbtrzdhu.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ytghkone.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wafwnvhw.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2nkuuuasv.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zlyanksi.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2fuwezdma.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2dvxuelfc.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2fbfalyoo.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2zxdnfgfc.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2fhwjjupn.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2tnhgmfwf.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2ebwutevj.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2lyjehasc.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tzbtreox.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2bdhygbjj.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2pdvxzkjo.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2vdoqpvgz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2hhcuqxdm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qfyerodo.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2lyjfdqto.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2unvcuciv.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2mbvnuael.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2oppwgzvb.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2vfgdwwyy.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2knbfjibc.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2xclzaxvi.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2gnisnoyz.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2wmhgdrcx.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2rtlwglle.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2abxzwdjf.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2inzcjvyt.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2qqkskwgw.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2zgtnykpo.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2xxoyqofq.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2pncrqxwc.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2jwzhicxm.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2afoskufr.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2tznuisga.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2rxsbepkw.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2exqsfzsx.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2emnkipuj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2yrjotmgs.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2yincwkaj.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2aglcvcde.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ttozpedz.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2jmwmmwjb.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2kbobvhuq.html

esac
来源：http://www.52xcode.cn/Article/details/gt2clefuidg.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2spjdbxzv.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2phuymsgc.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2clnwjkaf.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2xdzhfwyz.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2uywejsxr.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2quqrtaby.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2cbqoynsg.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jsazsgno.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2cucxbkuk.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2cdthednv.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2lnrjyswt.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ykqqydeq.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2fugmzyco.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2qyopggna.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2fmuhnqoo.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2gvdfcbxt.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2ryyxnori.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2tnvmxwps.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2kxqgrhtl.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2ridgojaf.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2cjkgqkem.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2oybqqqsc.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2prhumpzu.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2zxvjaoee.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2tytcmzbb.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2dntoarsy.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2rfvhskfa.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2bxyycrdb.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2wyvhwhov.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2ljgnxais.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2iggxgnrw.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2zppmsqum.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2entxstep.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2qpttwzps.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2gfobxzkj.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2kjbslepg.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2hvirfsnj.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2rlrqsana.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2krbkuxga.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cqpwpcet.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2ggocnqol.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2cujdbnpr.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2yubqvjzf.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2grtotsyr.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2nftvdigi.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2zguqmsmq.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2xkazouom.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2xbuqgvmy.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2uhumjjfc.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2gnxepmia.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2qcqtyibv.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2ikqqsefl.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2xwtngjrk.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2kjwjogrr.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2mjgympnu.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2uztoffvw.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2unorzmjs.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2nooppvab.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2igxsadam.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2jmdyahvr.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2svwjsygj.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2blowezhb.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2ntxnaxep.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2gjnszryf.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2yoedxiqm.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2pivejdgu.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2qdxktqrl.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2rbbnwnhp.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2doyuwrvp.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2wzotdlac.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2ebnozmww.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vgxurbqq.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2qcnrlfek.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ihdaiayd.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2ufxkbeae.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2ojnrdpae.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2wqdotzxg.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2welqxzew.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2rdfktjqz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2rmtclecy.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2ubjmqton.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rvhcenhf.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2wmkezpdn.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2jvicrtcb.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2slpiyqny.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2sqrdcejm.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2hljwqrni.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2vpfxzrou.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2lnmvarhd.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2rsdywvwu.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2gtvsmklr.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2clvystng.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2gfcjvjzq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2pcnglqxn.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2ijaldqfb.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2mralnjnl.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2yboahzqw.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2exlpsukv.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2lwhwktth.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2qaptsith.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2bbfpcjcu.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2cekhemmg.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2kerocgvd.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2alcozgoo.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2saitiscj.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2dduusiba.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2ohcxvdyv.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2fsdgqqeg.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2ftmddojx.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2jnucdhta.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2pcdstybz.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2qaetlgnv.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2uorlnsrj.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2vnuxizha.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2anspxlab.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2srjyuhyz.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2lndwnjdo.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2aiwtmhic.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2udxfzcht.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2vjmcpdak.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2yjwubudu.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2iltnqbua.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2klmmvrim.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2bpoicius.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2nrlrxgxm.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2tyciahbf.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2fkhwndrr.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2dednxuqb.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2gipuiegd.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2rvppiatd.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2ippqpqly.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2vmewakxq.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2aolqjbpa.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2ofeyrdyn.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2xmexshfz.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2okwrvpbp.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2lqrcqpfz.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2khzfhfeq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ypcrygyk.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2taaiqtvj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jqkioxbd.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ogrjvkps.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2hctyweiv.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2dixzpcmj.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2vorrwyfh.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2kknopnfo.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2wzowybxm.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2vibxjdog.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2cniktbbm.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2kfwancfy.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2rllfkeyj.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lmjqoihs.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2mmuavrur.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2zmhvytfn.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2lhksbksa.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2rvyoujim.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2tlbumajx.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2kycruawv.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2cnsztqcf.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2hgfhbzhu.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2bgcedtco.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2alcppkzf.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2tzzxwtwz.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2yqmmnjry.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2cvrodorf.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2mdhspeyg.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2ubgmgzbl.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2vrsunxzn.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2bxqwaqal.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2gytlzbky.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2hwzrpjcl.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2ygtilvwy.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2orcnlhge.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2dxwzdscl.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2hhyrivdt.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2wppewibj.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2xoncjhdh.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2qfkdhpwd.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2vjltbgnq.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2djsujhyb.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2fiqdfimz.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2auqypgpi.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2csorgzrx.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2htslwzke.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2vsfdyqdc.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2exhbvabl.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2zsdfxwao.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2bqulnwlp.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2nztgxvqq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2zchogzyu.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2gnhgoppm.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2cjkeejdt.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ksjumrer.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2fssbfqcc.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2iaizjojd.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2gedsrtwd.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2hyhanywi.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2yoixvasi.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2qtimdvre.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2easgkyjg.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2yxldahjc.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2hxbxqgsa.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2lirfreeh.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2kmdybjkw.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2anjvmqxx.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2haoxprce.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jykbpygr.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2utefiumt.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2pysulphe.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nnwuulvx.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2buptglxu.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2eflifvar.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2gdybofel.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2jeucgner.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2llxtbexo.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2wqhpsvxn.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2pgazvakp.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2hsrohoab.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lbgbhnnw.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2pqyomoqj.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2bqlfeopp.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2bqvcusox.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2pbpzdzbc.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2awdzeoyd.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2oyptdukz.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2hyhedysg.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ewczkgxi.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2qhxshfgq.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2dqvsandn.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2zccraipq.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2jnicfrxc.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2zhsnmtbc.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2hdgplnzs.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2yezfnupk.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ewfbpeoa.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2knegyntu.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2kqphiwqf.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2qzstcgcp.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2byffpwci.html


<!-- 参考信息 -->