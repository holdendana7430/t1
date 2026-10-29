代发 wailian999

[Q78] 当前时间
来源：http://wap.hesvh.cn/Article/details/grbzsiitu.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fehbvm.com/Article/details/glzrbbqbz.sHtML

[Q79] 字符串拼接
来源：http://baike.hesvh.cn/Article/details/gwvgzpobz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.zdbjq.cn/Article/details/gebarxmzs.sHtML

[Q80] 字符串截取
来源：http://read.share.zdbjq.cn/Article/details/gjzqmthek.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fehbvm.com/Article/details/gtmdhabye.sHtML

[Q81] 字符串替换
来源：http://blog.hesvh.cn/Article/details/gvlzjtrst.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gyrfrptjj.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.hesvh.cn/Article/details/gpywhltbn.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gjheokgez.sHtML

[Q83] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gpxhhwevc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gvxewobug.sHtML

[Q84] 去除首尾空格
来源：http://mobile.zdbjq.cn/Article/details/gtghziquq.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gxnpggbmf.sHtML

[Q85] 数值取整
来源：http://baike.fehbvm.com/Article/details/gdkkbnapn.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fehbvm.com/Article/details/gwdbdbhvd.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fehbvm.com/Article/details/gkhsghhlx.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.zdbjq.cn/Article/details/gmgufwdkm.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.zdbjq.cn/Article/details/gqdnnxoou.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.hesvh.cn/Article/details/gbgeoecxf.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fehbvm.com/Article/details/goazkolkr.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.zdbjq.cn/Article/details/gqaigaqpt.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fehbvm.com/Article/details/guscbhkzp.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gzggavbqg.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.hesvh.cn/Article/details/gazyazgxb.sHtML

[Q90] 生成序号列
来源：http://baike.zdbjq.cn/Article/details/gckrrkdhy.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.zdbjq.cn/Article/details/gbimjbmgl.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gxznmbbvg.sHtML

R. Bash 专题
来源：http://blog.hesvh.cn/Article/details/gaduodisw.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ggqnpjayi.sHtML

[R01] shebang 与严格模式
来源：http://blog.hesvh.cn/Article/details/gsapqvmca.sHtML

#!/usr/bin/env bash
来源：http://read.share.fehbvm.com/Article/details/gznkxpfrw.sHtML

set -euo pipefail
来源：http://blog.fehbvm.com/Article/details/gmiacbhqo.sHtML

[R02] 变量赋值与使用
来源：http://3g.zdbjq.cn/Article/details/gwmuskuix.sHtML

name="Tom"; echo "$name"
来源：http://baike.zdbjq.cn/Article/details/gncwyhsvh.sHtML

[R03] 只读变量
来源：http://blog.hesvh.cn/Article/details/gfycvauzj.sHtML

readonly PI=3.14
来源：http://blog.fehbvm.com/Article/details/gktnuhpvn.sHtML

[R04] 位置参数
来源：http://baike.fehbvm.com/Article/details/gnzgdshzf.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fehbvm.com/Article/details/gojfligdb.sHtML

[R05] 参数默认值
来源：http://www.share.hesvh.cn/Article/details/gegbjttei.sHtML

name="${1:-default}"
来源：http://m.share.zdbjq.cn/Article/details/glipovbto.sHtML

[R06] 判断命令是否存在
来源：http://wap.hesvh.cn/Article/details/gktwddlek.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/gclcnlqrw.sHtML

[R07] if 判断文件
来源：http://www.blog.fehbvm.com/Article/details/gspjzoxfv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.hesvh.cn/Article/details/gophzvohd.sHtML

[R08] 数值比较
来源：http://baike.fehbvm.com/Article/details/gaxjhjsdo.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.zdbjq.cn/Article/details/gvnjqbqon.sHtML

[R09] 字符串比较
来源：http://baike.zdbjq.cn/Article/details/gebhvwmjl.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.zdbjq.cn/Article/details/ghluzftyq.sHtML

[R10] 正则匹配
来源：http://www.share.zdbjq.cn/Article/details/gpcqelftb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gcediaagu.sHtML

[R11] case 多分支
来源：http://baike.hesvh.cn/Article/details/gflkuaukc.sHtML

case "$1" in
来源：http://www.share.fehbvm.com/Article/details/gfrxsvyny.sHtML

start) echo "启动" ;;
来源：http://www.blog.fehbvm.com/Article/details/gcabcymlx.sHtML

stop)  echo "停止" ;;
来源：http://m.share.hesvh.cn/Article/details/grynhzlpq.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.zdbjq.cn/Article/details/gwxhzpisy.sHtML

esac
来源：http://blog.zdbjq.cn/Article/details/gjeedxxnz.sHtML

[R12] for 遍历文件
来源：http://baike.fehbvm.com/Article/details/gaidcqtvw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.hesvh.cn/Article/details/gnqxofaje.sHtML

[R13] for 计数循环
来源：http://m.share.zdbjq.cn/Article/details/getqflqvj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/gewgpjbef.sHtML

[R14] C 风格 for
来源：http://blog.hesvh.cn/Article/details/giifvtrnx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/gkvqxwetz.sHtML

[R15] while 逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gblfnxkww.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fehbvm.com/Article/details/gxmmmqgcb.sHtML

[R16] until 等待条件
来源：http://m.share.fehbvm.com/Article/details/gscznyppw.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/gdfymobhn.sHtML

[R17] 数组定义与取值
来源：http://mobile.fehbvm.com/Article/details/gwsfejsjf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.zdbjq.cn/Article/details/gsqxrthlo.sHtML

[R18] 遍历数组
来源：http://www.m.share.zdbjq.cn/Article/details/ghkbsrcai.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.hesvh.cn/Article/details/gopfeetis.sHtML

[R19] 数组长度
来源：http://blog.hesvh.cn/Article/details/gxzwpeczj.sHtML

echo "${#arr[@]}"
来源：http://blog.hesvh.cn/Article/details/glyxccrdk.sHtML

[R20] 关联数组（字典）
来源：http://read.share.zdbjq.cn/Article/details/gpmmbnnro.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.zdbjq.cn/Article/details/gpfbsscht.sHtML

[R21] 字符串长度
来源：http://www.share.fehbvm.com/Article/details/gvvekcgjs.sHtML

echo "${#s}"
来源：http://www.share.zdbjq.cn/Article/details/gcqkodwgp.sHtML

[R22] 截取子串
来源：http://3g.hesvh.cn/Article/details/gywagswfz.sHtML

echo "${s:0:5}"
来源：http://baike.hesvh.cn/Article/details/gckojczag.sHtML

[R23] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/gvxllnipd.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.hesvh.cn/Article/details/gnnjahgtt.sHtML

[R24] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/ghciqdwnw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fehbvm.com/Article/details/gcltrknwu.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fehbvm.com/Article/details/gacclhuex.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.hesvh.cn/Article/details/grpdwbfry.sHtML

[R26] 命令替换
来源：http://blog.zdbjq.cn/Article/details/gohplafvw.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.hesvh.cn/Article/details/gisskbbfk.sHtML

[R27] 算术展开
来源：http://www.m.share.hesvh.cn/Article/details/gceitaqhi.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fehbvm.com/Article/details/gltdbgylj.sHtML

[R28] 浮点运算
来源：http://3g.zdbjq.cn/Article/details/giphyfkeg.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fehbvm.com/Article/details/gyyovwzro.sHtML

[R29] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/gtrnkwvll.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fehbvm.com/Article/details/gluebzqqf.sHtML

[R30] 函数返回状态码
来源：http://baike.fehbvm.com/Article/details/ggcwuvujc.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fehbvm.com/Article/details/gcjfbesgo.sHtML

[R31] 局部变量
来源：http://m.share.hesvh.cn/Article/details/gydolobci.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.hesvh.cn/Article/details/gxzyjtjru.sHtML

[R32] 参数个数校验
来源：http://blog.fehbvm.com/Article/details/gqimqtwqu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/ghtpdgjgh.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.hesvh.cn/Article/details/gyatuymyt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.zdbjq.cn/Article/details/gmlblvyun.sHtML

[R34] 退出时清理
来源：http://wap.zdbjq.cn/Article/details/gctpnwbal.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/gcpauwssh.sHtML

[R35] 后台执行并等待
来源：http://www.blog.hesvh.cn/Article/details/grbrlntlq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.hesvh.cn/Article/details/gmtmwfjhs.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.hesvh.cn/Article/details/gblifnlch.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.zdbjq.cn/Article/details/gvlqmvwdi.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fehbvm.com/Article/details/gopujwvck.sHtML

files=$(ls -1)
来源：http://read.share.hesvh.cn/Article/details/grzfkwrve.sHtML

[R38] 管道串联
来源：http://read.share.hesvh.cn/Article/details/gqbxvuztc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fehbvm.com/Article/details/gtrwoqyev.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.hesvh.cn/Article/details/gyjounstu.sHtML

cmd > out.log 2>&1
来源：http://www.share.zdbjq.cn/Article/details/gpksonhpv.sHtML

[R40] 追加写日志
来源：http://m.share.hesvh.cn/Article/details/gghaybjce.sHtML

echo "log" >> out.log
来源：http://3g.fehbvm.com/Article/details/gfoivjooz.sHtML

[R41] 丢弃输出
来源：http://read.share.hesvh.cn/Article/details/gynhewvls.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.hesvh.cn/Article/details/gawyzffao.sHtML

[R42] 输入重定向
来源：http://baike.fehbvm.com/Article/details/gqwckpwym.sHtML

wc -l < a.txt
来源：http://mobile.hesvh.cn/Article/details/ghkyqagqm.sHtML

[R43] 按名字查找文件
来源：http://mobile.zdbjq.cn/Article/details/gutnphfnd.sHtML

find . -name "*.log" -type f
来源：http://baike.hesvh.cn/Article/details/gymxrjkbr.sHtML

[R44] 按修改时间查找
来源：http://baike.hesvh.cn/Article/details/gimegqzzd.sHtML

find . -mtime -7 -type f
来源：http://blog.zdbjq.cn/Article/details/gtzfuyhit.sHtML

[R45] 批量删除
来源：http://www.share.hesvh.cn/Article/details/gusqyxouf.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.zdbjq.cn/Article/details/gxvlrtkxa.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.zdbjq.cn/Article/details/glytcasdu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fehbvm.com/Article/details/gdowznvuc.sHtML

[R47] sed 单行替换
来源：http://www.share.fehbvm.com/Article/details/gkwfkysxq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gedhpfjoi.sHtML

[R48] awk 取指定列
来源：http://3g.hesvh.cn/Article/details/gaoflhnxh.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.hesvh.cn/Article/details/gawxtzhgp.sHtML

[R49] awk 带条件
来源：http://wap.zdbjq.cn/Article/details/guoqhkolw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fehbvm.com/Article/details/gfskphovl.sHtML

[R50] awk 求和
来源：http://baike.hesvh.cn/Article/details/gtugloecz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.zdbjq.cn/Article/details/gnqzmprcc.sHtML

[R51] 排序去重取前几
来源：http://3g.zdbjq.cn/Article/details/gqsuvcpzq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.hesvh.cn/Article/details/gwhfupgdj.sHtML

[R52] 统计行数
来源：http://mobile.hesvh.cn/Article/details/gofqxxlso.sHtML

wc -l a.txt
来源：http://blog.hesvh.cn/Article/details/gcpwxefwu.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.hesvh.cn/Article/details/gzhouezqc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.hesvh.cn/Article/details/grufsiapr.sHtML

[R54] 比较两个文件
来源：http://read.share.fehbvm.com/Article/details/gimddblqd.sHtML

diff a.txt b.txt
来源：http://mobile.fehbvm.com/Article/details/gbqejzjnh.sHtML

[R55] 压缩与解压
来源：http://wap.hesvh.cn/Article/details/gymbeoubb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fehbvm.com/Article/details/glmmjggwj.sHtML

[R56] 远程拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gxezhbglv.sHtML

scp file user@host:/path/
来源：http://baike.zdbjq.cn/Article/details/geikorlqh.sHtML

[R57] 远程执行命令
来源：http://read.share.zdbjq.cn/Article/details/giajgdafv.sHtML

ssh user@host 'uptime'
来源：http://mobile.zdbjq.cn/Article/details/gbulhtmyc.sHtML

[R58] 下载文件
来源：http://www.share.fehbvm.com/Article/details/gxghezewh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.hesvh.cn/Article/details/gncxawhqg.sHtML

[R59] 发 POST JSON
来源：http://read.share.fehbvm.com/Article/details/gtwncehpw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.zdbjq.cn/Article/details/gvltygpnp.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/ggpsomalw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.zdbjq.cn/Article/details/gkhbnyxmk.sHtML

[R61] 磁盘占用
来源：http://wap.hesvh.cn/Article/details/gvyqopeku.sHtML

df -h;  du -sh *
来源：http://www.share.zdbjq.cn/Article/details/gojcarwio.sHtML

[R62] 找最占空间的文件
来源：http://wap.zdbjq.cn/Article/details/gskfdzoop.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fehbvm.com/Article/details/gofryndwg.sHtML

[R63] 内存与进程
来源：http://3g.zdbjq.cn/Article/details/gklikxskq.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.zdbjq.cn/Article/details/gzcbatksk.sHtML

[R64] 结束进程
来源：http://www.share.fehbvm.com/Article/details/gevjxtiqo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.hesvh.cn/Article/details/gbmdzqyzz.sHtML

[R65] 查看端口占用
来源：http://baike.hesvh.cn/Article/details/gjzkgibsz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fehbvm.com/Article/details/gwqhcewra.sHtML

[R66] 定时任务
来源：http://wap.zdbjq.cn/Article/details/gpjvnmrjv.sHtML

crontab -e;  crontab -l
来源：http://read.share.zdbjq.cn/Article/details/gtdrkbdwf.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.hesvh.cn/Article/details/gybfhcqeu.sHtML

openssl rand -hex 16
来源：http://3g.zdbjq.cn/Article/details/gxrcftyrf.sHtML

[R68] 计算文件校验值
来源：http://www.blog.hesvh.cn/Article/details/grkykvqkz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.zdbjq.cn/Article/details/gjpcbvfxp.sHtML

[R69] 生成随机密码
来源：http://baike.zdbjq.cn/Article/details/gvcrhcqsa.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.hesvh.cn/Article/details/gxsmklkxb.sHtML

[R70] 时间戳与互转
来源：http://mobile.fehbvm.com/Article/details/ggbpfbpip.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fehbvm.com/Article/details/gafurtywt.sHtML

[R71] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/glhoqjskc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.hesvh.cn/Article/details/gvrljhqxo.sHtML

[R72] 等待端口就绪
来源：http://blog.fehbvm.com/Article/details/ggmcdiapy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/gvnzahmfa.sHtML

[R73] 分割大日志
来源：http://blog.hesvh.cn/Article/details/gsptjcgns.sHtML

split -l 1000 big.log part_
来源：http://mobile.hesvh.cn/Article/details/gbocquxui.sHtML

[R74] 批量重命名
来源：http://wap.hesvh.cn/Article/details/gpaphilvx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.zdbjq.cn/Article/details/gxvaaaims.sHtML

[R75] 导出环境变量
来源：http://www.share.fehbvm.com/Article/details/gqfetuvqw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fehbvm.com/Article/details/gtfclbxkl.sHtML

[R76] 使用临时文件
来源：http://3g.zdbjq.cn/Article/details/gcszkokul.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/grlodozsb.sHtML

[R77] 读取用户输入
来源：http://www.share.fehbvm.com/Article/details/gywcdaqay.sHtML

read -rp "请输入: " ans
来源：http://blog.fehbvm.com/Article/details/gakitqiib.sHtML

[R78] 交互式菜单
来源：http://www.m.share.zdbjq.cn/Article/details/gaftcfrma.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fehbvm.com/Article/details/gxxnclgfx.sHtML

[R79] 解析命令行选项
来源：http://www.share.fehbvm.com/Article/details/gwviurvvf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.zdbjq.cn/Article/details/gijaqgcpd.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fehbvm.com/Article/details/gctqhfnzd.sHtML

time ./run.sh
来源：http://www.blog.zdbjq.cn/Article/details/gwcpzacmj.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gqfsvofij.sHtML

S. C / C++ 专题
来源：http://mobile.fehbvm.com/Article/details/gauxokamb.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gcbgsapbc.sHtML

[S01] C：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/ghmyidffu.sHtML

#include <stdio.h>
来源：http://baike.zdbjq.cn/Article/details/gwrqmmzjc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.zdbjq.cn/Article/details/gyshreaer.sHtML

[S02] C：变量与格式化输出
来源：http://baike.hesvh.cn/Article/details/galpjomgz.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.hesvh.cn/Article/details/gwkjbxjkj.sHtML

[S03] C：读入整数
来源：http://www.blog.hesvh.cn/Article/details/grpsjndka.sHtML

int x; scanf("%d", &x);
来源：http://m.share.zdbjq.cn/Article/details/gtdrkvgks.sHtML

[S04] C：字符串复制
来源：http://www.blog.fehbvm.com/Article/details/ghidfiilv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.hesvh.cn/Article/details/gjpcnchim.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/gkdqrtjfc.sHtML

strlen(s)
来源：http://wap.hesvh.cn/Article/details/gslfxmznb.sHtML

[S06] C：字符串比较
来源：http://wap.hesvh.cn/Article/details/gkqoktkqe.sHtML

strcmp(a, b) == 0
来源：http://mobile.hesvh.cn/Article/details/gtmrcuprg.sHtML

[S07] C：数组遍历求和
来源：http://wap.fehbvm.com/Article/details/glpxsyhrp.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fehbvm.com/Article/details/ghzhegeyv.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.hesvh.cn/Article/details/guulfcapa.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fehbvm.com/Article/details/gbjzqzbbt.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fehbvm.com/Article/details/gsexfzzul.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.hesvh.cn/Article/details/gdrsatznx.sHtML

[S10] C：指针与解引用
来源：http://wap.zdbjq.cn/Article/details/gwxgweqdt.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.zdbjq.cn/Article/details/geripvdrv.sHtML

[S11] C：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gnrecsahw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.hesvh.cn/Article/details/grwetdhdx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.hesvh.cn/Article/details/gixxtyvzw.sHtML

fclose(f);
来源：http://blog.fehbvm.com/Article/details/gvzxblkvv.sHtML

[S12] C：写文件
来源：http://3g.zdbjq.cn/Article/details/gzjcmwfxa.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/gymeexbws.sHtML

[S13] C：宏定义
来源：http://www.blog.fehbvm.com/Article/details/gqilswqub.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.hesvh.cn/Article/details/grjycjrju.sHtML

[S14] C：枚举
来源：http://mobile.hesvh.cn/Article/details/gseiazbxw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.zdbjq.cn/Article/details/gjgbftvdf.sHtML

[S15] C：类型转换
来源：http://blog.hesvh.cn/Article/details/gmpevornf.sHtML

(double) a / b
来源：http://read.share.hesvh.cn/Article/details/gqlhfmfxn.sHtML

[S16] C：位操作置位
来源：http://www.share.hesvh.cn/Article/details/ggauvlurz.sHtML

x |= (1 << 3);
来源：http://www.m.share.hesvh.cn/Article/details/gzkaokfyf.sHtML

[S17] C：安全拼接字符串
来源：http://wap.hesvh.cn/Article/details/ganqlblbs.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.zdbjq.cn/Article/details/gdujecejt.sHtML

[S18] C：命令行参数
来源：http://mobile.fehbvm.com/Article/details/ghbpqboew.sHtML

int main(int argc, char **argv)
来源：http://www.share.zdbjq.cn/Article/details/glrcnqtoz.sHtML

[S19] C：快速排序
来源：http://m.share.fehbvm.com/Article/details/grwrwyswo.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/gsctizurs.sHtML

[S20] C：二分查找
来源：http://wap.fehbvm.com/Article/details/gcvdzylxf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/glnbnxcoa.sHtML

[S21] C：字符类别判断
来源：http://baike.hesvh.cn/Article/details/growmzjiz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.zdbjq.cn/Article/details/gycziibse.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/gbinenqoc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.zdbjq.cn/Article/details/gwoxyprsw.sHtML

[S23] C：随机数
来源：http://www.share.fehbvm.com/Article/details/geosiddmv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.zdbjq.cn/Article/details/gisxozdzr.sHtML

[S24] C：获取本地时间
来源：http://www.share.zdbjq.cn/Article/details/gmcvfmclv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.zdbjq.cn/Article/details/gmvpjudhp.sHtML

[S25] C：内存拷贝
来源：http://www.blog.hesvh.cn/Article/details/gamnelgyg.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fehbvm.com/Article/details/gfyvuuavp.sHtML

[S26] C：内存清零
来源：http://wap.zdbjq.cn/Article/details/gsjcxqrpe.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.zdbjq.cn/Article/details/gijkehdbs.sHtML

[S27] C：定义常量
来源：http://baike.zdbjq.cn/Article/details/gabkewube.sHtML

const double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gvozqcrlb.sHtML

[S28] C：静态变量
来源：http://mobile.zdbjq.cn/Article/details/gkrlwmfgp.sHtML

static int counter = 0;
来源：http://wap.fehbvm.com/Article/details/gvbjrgfvc.sHtML

[S29] C：变参函数
来源：http://www.m.share.hesvh.cn/Article/details/gdfgslnhy.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fehbvm.com/Article/details/ghjimxriw.sHtML

[S30] C：头文件保护
来源：http://mobile.hesvh.cn/Article/details/ghpujrngh.sHtML

#ifndef X_H
来源：http://m.share.fehbvm.com/Article/details/gllmfptps.sHtML

#define X_H
来源：http://www.share.zdbjq.cn/Article/details/gchjhegiu.sHtML

#endif
来源：http://m.share.zdbjq.cn/Article/details/gbthkdulu.sHtML

[S31] C++：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gdmrboivs.sHtML

#include <iostream>
来源：http://wap.hesvh.cn/Article/details/gvvisgssr.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.hesvh.cn/Article/details/ghqdranjj.sHtML

[S32] C++：字符串
来源：http://blog.fehbvm.com/Article/details/gkszhcdar.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fehbvm.com/Article/details/gjbskvffq.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.hesvh.cn/Article/details/gxgysinox.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.hesvh.cn/Article/details/gejhvyipc.sHtML

[S34] C++：遍历 vector
来源：http://baike.zdbjq.cn/Article/details/gyzlqgvfl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fehbvm.com/Article/details/gnieuaoqo.sHtML

[S35] C++：map
来源：http://baike.hesvh.cn/Article/details/gptyzfrxf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/gghdovzob.sHtML

[S36] C++：unordered_map
来源：http://blog.hesvh.cn/Article/details/gqnezpwux.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/gmzketqwh.sHtML

[S37] C++：set
来源：http://wap.fehbvm.com/Article/details/gamlfacjo.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fehbvm.com/Article/details/gatpfhowr.sHtML

[S38] C++：排序
来源：http://read.share.hesvh.cn/Article/details/gsnpcjmdy.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fehbvm.com/Article/details/giwnqrgbq.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.zdbjq.cn/Article/details/ghpnirhxe.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.hesvh.cn/Article/details/gmrxhhknz.sHtML

[S40] C++：查找元素
来源：http://www.share.zdbjq.cn/Article/details/gtukaysfn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gpwhnkzpc.sHtML

[S41] C++：类与构造函数
来源：http://read.share.hesvh.cn/Article/details/gdhzdttur.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.zdbjq.cn/Article/details/gyomnezis.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.zdbjq.cn/Article/details/geuabkiol.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.zdbjq.cn/Article/details/gqszwcidj.sHtML

[S43] C++：智能指针
来源：http://www.blog.hesvh.cn/Article/details/ghjjntcdl.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.hesvh.cn/Article/details/gsnbqqhvz.sHtML

[S44] C++：引用传参
来源：http://www.share.hesvh.cn/Article/details/gpbowyogn.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.zdbjq.cn/Article/details/gopcjdgbb.sHtML

[S45] C++：lambda
来源：http://wap.hesvh.cn/Article/details/glvdeqpvo.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fehbvm.com/Article/details/gblaperdw.sHtML

[S46] C++：函数模板
来源：http://www.m.share.zdbjq.cn/Article/details/gprrsrfjm.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fehbvm.com/Article/details/gdumxhpmp.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fehbvm.com/Article/details/giokiiygq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fehbvm.com/Article/details/gmjsvbwcy.sHtML

[S48] C++：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gddcldpzc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fehbvm.com/Article/details/gzfhsmuni.sHtML


<!-- 参考信息 -->