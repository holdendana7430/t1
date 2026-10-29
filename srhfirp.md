代发 wailian999

[Q78] 当前时间
来源：http://3g.hesvh.cn/Article/details/gxvlywkhf.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.hesvh.cn/Article/details/gqkvbffnd.sHtML

[Q79] 字符串拼接
来源：http://wap.hesvh.cn/Article/details/gowohjgvr.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.hesvh.cn/Article/details/gbrsxlsbq.sHtML

[Q80] 字符串截取
来源：http://m.share.hesvh.cn/Article/details/gjkdjpuaf.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gpkbdpmas.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/gxilmvrjb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gjqzbuhhc.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.zdbjq.cn/Article/details/gzjntcphy.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gkvlpxblp.sHtML

[Q83] 大小写转换
来源：http://blog.fehbvm.com/Article/details/ggtpoejvs.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/grmsedmou.sHtML

[Q84] 去除首尾空格
来源：http://3g.zdbjq.cn/Article/details/gormycnjj.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/ggejnmdhf.sHtML

[Q85] 数值取整
来源：http://wap.fehbvm.com/Article/details/gbitjsqxz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fehbvm.com/Article/details/gbytybsmx.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fehbvm.com/Article/details/grxydzrdm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fehbvm.com/Article/details/gmqfssucf.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.hesvh.cn/Article/details/gcweugqge.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fehbvm.com/Article/details/gbjdbjnep.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fehbvm.com/Article/details/gdiqbxogk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.hesvh.cn/Article/details/gwlaejtff.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.hesvh.cn/Article/details/gzmhielna.sHtML

[Q89] 判断表是否存在
来源：http://wap.zdbjq.cn/Article/details/gjoruezgz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.zdbjq.cn/Article/details/ginjozhaj.sHtML

[Q90] 生成序号列
来源：http://blog.fehbvm.com/Article/details/gyraeavuu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fehbvm.com/Article/details/geaenfsqp.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gwqjdwlhp.sHtML

R. Bash 专题
来源：http://m.share.hesvh.cn/Article/details/gntkapqlj.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gqpnypdin.sHtML

[R01] shebang 与严格模式
来源：http://blog.fehbvm.com/Article/details/gubfrhulz.sHtML

#!/usr/bin/env bash
来源：http://blog.hesvh.cn/Article/details/giqckpnsa.sHtML

set -euo pipefail
来源：http://m.share.hesvh.cn/Article/details/gyaxoxwkv.sHtML

[R02] 变量赋值与使用
来源：http://baike.hesvh.cn/Article/details/gfompklob.sHtML

name="Tom"; echo "$name"
来源：http://3g.fehbvm.com/Article/details/gnpysxlib.sHtML

[R03] 只读变量
来源：http://www.share.fehbvm.com/Article/details/gnbnokcrz.sHtML

readonly PI=3.14
来源：http://m.share.zdbjq.cn/Article/details/ggvmigwfh.sHtML

[R04] 位置参数
来源：http://m.share.zdbjq.cn/Article/details/gnsvbesot.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.hesvh.cn/Article/details/gzakgrsuh.sHtML

[R05] 参数默认值
来源：http://www.m.share.fehbvm.com/Article/details/gtxokcupv.sHtML

name="${1:-default}"
来源：http://3g.fehbvm.com/Article/details/geaybuytk.sHtML

[R06] 判断命令是否存在
来源：http://blog.zdbjq.cn/Article/details/gpiznkpnz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/gzuusaisq.sHtML

[R07] if 判断文件
来源：http://read.share.zdbjq.cn/Article/details/gxxthyazq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gyluvzuqw.sHtML

[R08] 数值比较
来源：http://mobile.zdbjq.cn/Article/details/gooteqgqj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.hesvh.cn/Article/details/geupnhrks.sHtML

[R09] 字符串比较
来源：http://wap.fehbvm.com/Article/details/gvxnywzyc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.zdbjq.cn/Article/details/gmdhkllux.sHtML

[R10] 正则匹配
来源：http://m.share.hesvh.cn/Article/details/gtbfeprhw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fehbvm.com/Article/details/gatmxonwo.sHtML

[R11] case 多分支
来源：http://www.blog.fehbvm.com/Article/details/gsurxpqvn.sHtML

case "$1" in
来源：http://baike.hesvh.cn/Article/details/gxdodximn.sHtML

start) echo "启动" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gdwpztdpj.sHtML

stop)  echo "停止" ;;
来源：http://mobile.zdbjq.cn/Article/details/gazujlbcs.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.hesvh.cn/Article/details/gnrlzztmp.sHtML

esac
来源：http://blog.zdbjq.cn/Article/details/ggrkhpplm.sHtML

[R12] for 遍历文件
来源：http://www.share.hesvh.cn/Article/details/ggxfugseu.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fehbvm.com/Article/details/glhjdghvy.sHtML

[R13] for 计数循环
来源：http://blog.hesvh.cn/Article/details/gooopxalz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gzidmnyrt.sHtML

[R14] C 风格 for
来源：http://m.share.zdbjq.cn/Article/details/gmqasuxto.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/gfnrnzjer.sHtML

[R15] while 逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/ggfgwngjh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.hesvh.cn/Article/details/gylbweiyv.sHtML

[R16] until 等待条件
来源：http://blog.hesvh.cn/Article/details/gwfwzigze.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/gszkjwaaf.sHtML

[R17] 数组定义与取值
来源：http://wap.zdbjq.cn/Article/details/gvojswmmz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fehbvm.com/Article/details/gccbtlkvy.sHtML

[R18] 遍历数组
来源：http://www.share.zdbjq.cn/Article/details/gqeunshgm.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fehbvm.com/Article/details/gkkicrwjj.sHtML

[R19] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/gqisumjya.sHtML

echo "${#arr[@]}"
来源：http://mobile.zdbjq.cn/Article/details/gasfrpqpa.sHtML

[R20] 关联数组（字典）
来源：http://blog.fehbvm.com/Article/details/gfohaqwcm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fehbvm.com/Article/details/goxmjwqrh.sHtML

[R21] 字符串长度
来源：http://3g.hesvh.cn/Article/details/gqdefawia.sHtML

echo "${#s}"
来源：http://baike.fehbvm.com/Article/details/gqwmuboox.sHtML

[R22] 截取子串
来源：http://wap.hesvh.cn/Article/details/gkohficue.sHtML

echo "${s:0:5}"
来源：http://3g.fehbvm.com/Article/details/gwgmsivrc.sHtML

[R23] 字符串替换
来源：http://blog.hesvh.cn/Article/details/gzhitmzni.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.hesvh.cn/Article/details/gqtketyga.sHtML

[R24] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/gytmaquud.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.zdbjq.cn/Article/details/gputrvtfp.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fehbvm.com/Article/details/gsdaahabo.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.hesvh.cn/Article/details/gyakkewvr.sHtML

[R26] 命令替换
来源：http://mobile.fehbvm.com/Article/details/gajmiskws.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.hesvh.cn/Article/details/gjbqjwigq.sHtML

[R27] 算术展开
来源：http://mobile.hesvh.cn/Article/details/gikkchkwl.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fehbvm.com/Article/details/gleqfhwjj.sHtML

[R28] 浮点运算
来源：http://baike.hesvh.cn/Article/details/gpbexeaju.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.hesvh.cn/Article/details/glmospcad.sHtML

[R29] 定义函数
来源：http://www.share.zdbjq.cn/Article/details/gfstpmwcp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fehbvm.com/Article/details/gnzhtxcwa.sHtML

[R30] 函数返回状态码
来源：http://m.share.hesvh.cn/Article/details/gceckiodl.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.hesvh.cn/Article/details/gypedstii.sHtML

[R31] 局部变量
来源：http://read.share.zdbjq.cn/Article/details/gbxxouqkv.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fehbvm.com/Article/details/ghcjzdhec.sHtML

[R32] 参数个数校验
来源：http://mobile.fehbvm.com/Article/details/gbbfezszx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/gymxjlpfw.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.hesvh.cn/Article/details/gwfrbwtdg.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fehbvm.com/Article/details/gmrcuflvi.sHtML

[R34] 退出时清理
来源：http://www.m.share.hesvh.cn/Article/details/gazdnmuez.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/gydcmnzbg.sHtML

[R35] 后台执行并等待
来源：http://read.share.zdbjq.cn/Article/details/gylzmvkhj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fehbvm.com/Article/details/gysohepfb.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.hesvh.cn/Article/details/gfsjoneyd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fehbvm.com/Article/details/gmdfvnpst.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fehbvm.com/Article/details/gtcizesrm.sHtML

files=$(ls -1)
来源：http://www.share.fehbvm.com/Article/details/gmslsxqbc.sHtML

[R38] 管道串联
来源：http://mobile.hesvh.cn/Article/details/grbgvsudb.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.hesvh.cn/Article/details/glaxapcvo.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.zdbjq.cn/Article/details/gfproiwof.sHtML

cmd > out.log 2>&1
来源：http://mobile.hesvh.cn/Article/details/gfxzhmwry.sHtML

[R40] 追加写日志
来源：http://wap.hesvh.cn/Article/details/gncqgaibh.sHtML

echo "log" >> out.log
来源：http://baike.fehbvm.com/Article/details/gcgeaolml.sHtML

[R41] 丢弃输出
来源：http://mobile.fehbvm.com/Article/details/gawcrzdzg.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fehbvm.com/Article/details/gmgrxlrsw.sHtML

[R42] 输入重定向
来源：http://baike.hesvh.cn/Article/details/gmfkseeen.sHtML

wc -l < a.txt
来源：http://www.blog.zdbjq.cn/Article/details/ghcyhuvob.sHtML

[R43] 按名字查找文件
来源：http://blog.zdbjq.cn/Article/details/geavpsnwk.sHtML

find . -name "*.log" -type f
来源：http://mobile.zdbjq.cn/Article/details/grvojlvco.sHtML

[R44] 按修改时间查找
来源：http://baike.fehbvm.com/Article/details/gxlrhzcuc.sHtML

find . -mtime -7 -type f
来源：http://m.share.hesvh.cn/Article/details/gdcmklkmp.sHtML

[R45] 批量删除
来源：http://wap.zdbjq.cn/Article/details/gochtgiju.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fehbvm.com/Article/details/gdlsbfpby.sHtML

[R46] 递归替换文件内容
来源：http://mobile.zdbjq.cn/Article/details/gmhjnqona.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.zdbjq.cn/Article/details/grgimeqcq.sHtML

[R47] sed 单行替换
来源：http://read.share.fehbvm.com/Article/details/gbmyfawxt.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gvdvvsmen.sHtML

[R48] awk 取指定列
来源：http://mobile.fehbvm.com/Article/details/gujihvrld.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gggkunejf.sHtML

[R49] awk 带条件
来源：http://www.blog.hesvh.cn/Article/details/gjgkthxnm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.hesvh.cn/Article/details/gcngxrobu.sHtML

[R50] awk 求和
来源：http://www.share.hesvh.cn/Article/details/gilbuyymi.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/guafoxfbt.sHtML

[R51] 排序去重取前几
来源：http://baike.hesvh.cn/Article/details/gkgdvsisn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.zdbjq.cn/Article/details/gfurbwspa.sHtML

[R52] 统计行数
来源：http://read.share.zdbjq.cn/Article/details/gkamhpqde.sHtML

wc -l a.txt
来源：http://wap.fehbvm.com/Article/details/gjswdrkwt.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.hesvh.cn/Article/details/gcgxguipe.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.zdbjq.cn/Article/details/gwfolfbti.sHtML

[R54] 比较两个文件
来源：http://blog.zdbjq.cn/Article/details/gfqtkxdti.sHtML

diff a.txt b.txt
来源：http://read.share.zdbjq.cn/Article/details/guyhfgpcc.sHtML

[R55] 压缩与解压
来源：http://baike.hesvh.cn/Article/details/gwotzkuyw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fehbvm.com/Article/details/glldujssi.sHtML

[R56] 远程拷贝
来源：http://www.share.fehbvm.com/Article/details/ggxjfcqng.sHtML

scp file user@host:/path/
来源：http://baike.zdbjq.cn/Article/details/gvmhwjnph.sHtML

[R57] 远程执行命令
来源：http://m.share.hesvh.cn/Article/details/gbrjlooup.sHtML

ssh user@host 'uptime'
来源：http://baike.fehbvm.com/Article/details/gjorddmah.sHtML

[R58] 下载文件
来源：http://wap.hesvh.cn/Article/details/gxqbuuhec.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fehbvm.com/Article/details/gmotldxxd.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fehbvm.com/Article/details/gdadhmbyu.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.hesvh.cn/Article/details/gbthktzoj.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/geulvlgcc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.zdbjq.cn/Article/details/gniqspvyo.sHtML

[R61] 磁盘占用
来源：http://mobile.zdbjq.cn/Article/details/glmwpcloo.sHtML

df -h;  du -sh *
来源：http://mobile.zdbjq.cn/Article/details/gozvafzyu.sHtML

[R62] 找最占空间的文件
来源：http://wap.hesvh.cn/Article/details/gdkmnwxku.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fehbvm.com/Article/details/guamqilnv.sHtML

[R63] 内存与进程
来源：http://www.blog.fehbvm.com/Article/details/gtermfxvx.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.hesvh.cn/Article/details/gpwhlaxuq.sHtML

[R64] 结束进程
来源：http://baike.zdbjq.cn/Article/details/gavsoqkin.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.hesvh.cn/Article/details/gtzhkzqoo.sHtML

[R65] 查看端口占用
来源：http://wap.zdbjq.cn/Article/details/guukbgsxr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.hesvh.cn/Article/details/gtduqzzcw.sHtML

[R66] 定时任务
来源：http://baike.fehbvm.com/Article/details/gofifvmud.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fehbvm.com/Article/details/ghfukmfgc.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.zdbjq.cn/Article/details/gkyqmoqte.sHtML

openssl rand -hex 16
来源：http://wap.hesvh.cn/Article/details/gwoaanzys.sHtML

[R68] 计算文件校验值
来源：http://3g.fehbvm.com/Article/details/gbmznvyuu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fehbvm.com/Article/details/gpacbskiq.sHtML

[R69] 生成随机密码
来源：http://blog.fehbvm.com/Article/details/gplvlqpto.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.zdbjq.cn/Article/details/gircfmudu.sHtML

[R70] 时间戳与互转
来源：http://wap.zdbjq.cn/Article/details/gadvqupvu.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.hesvh.cn/Article/details/gjzcahhwh.sHtML

[R71] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gnbpekglp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.zdbjq.cn/Article/details/gmytmxvrx.sHtML

[R72] 等待端口就绪
来源：http://blog.zdbjq.cn/Article/details/gqtjhguhi.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gjweetypw.sHtML

[R73] 分割大日志
来源：http://read.share.zdbjq.cn/Article/details/gdwakhgot.sHtML

split -l 1000 big.log part_
来源：http://m.share.hesvh.cn/Article/details/gtzhdxjda.sHtML

[R74] 批量重命名
来源：http://www.share.zdbjq.cn/Article/details/gtsduywhz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fehbvm.com/Article/details/gimairwts.sHtML

[R75] 导出环境变量
来源：http://www.share.hesvh.cn/Article/details/gscgwbohj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.hesvh.cn/Article/details/gfuvgvjru.sHtML

[R76] 使用临时文件
来源：http://blog.fehbvm.com/Article/details/gyyvypjjm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/gglijzgnl.sHtML

[R77] 读取用户输入
来源：http://read.share.hesvh.cn/Article/details/gommvudjq.sHtML

read -rp "请输入: " ans
来源：http://m.share.zdbjq.cn/Article/details/grtwdarmr.sHtML

[R78] 交互式菜单
来源：http://www.blog.zdbjq.cn/Article/details/gaoxdtuey.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.zdbjq.cn/Article/details/gfigzuwdv.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fehbvm.com/Article/details/gxmhfdqat.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fehbvm.com/Article/details/garaayfck.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.hesvh.cn/Article/details/gcxvdydbp.sHtML

time ./run.sh
来源：http://www.share.fehbvm.com/Article/details/gbvrjuvun.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gnmgishpb.sHtML

S. C / C++ 专题
来源：http://blog.zdbjq.cn/Article/details/goxvovffi.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gxfbbazlw.sHtML

[S01] C：Hello World
来源：http://blog.fehbvm.com/Article/details/gypseeiye.sHtML

#include <stdio.h>
来源：http://www.m.share.zdbjq.cn/Article/details/gkfdntbeh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.hesvh.cn/Article/details/gcquvrvht.sHtML

[S02] C：变量与格式化输出
来源：http://baike.zdbjq.cn/Article/details/gcwkviyho.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fehbvm.com/Article/details/gvhhqdoum.sHtML

[S03] C：读入整数
来源：http://wap.hesvh.cn/Article/details/guoawlwhd.sHtML

int x; scanf("%d", &x);
来源：http://mobile.zdbjq.cn/Article/details/gmnznwkvo.sHtML

[S04] C：字符串复制
来源：http://www.share.fehbvm.com/Article/details/gqqtbditf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fehbvm.com/Article/details/gwwqmolnr.sHtML

[S05] C：字符串长度
来源：http://www.share.hesvh.cn/Article/details/gwuktctdk.sHtML

strlen(s)
来源：http://3g.hesvh.cn/Article/details/ghrnhduqi.sHtML

[S06] C：字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/gttbfqodz.sHtML

strcmp(a, b) == 0
来源：http://read.share.fehbvm.com/Article/details/gxjbozubt.sHtML

[S07] C：数组遍历求和
来源：http://3g.fehbvm.com/Article/details/ggwntlmfw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.zdbjq.cn/Article/details/gtgvwriwe.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fehbvm.com/Article/details/gjcfvgukm.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.hesvh.cn/Article/details/gkcbcgaqq.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.zdbjq.cn/Article/details/ggsmftmjg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fehbvm.com/Article/details/gknrbzfzk.sHtML

[S10] C：指针与解引用
来源：http://read.share.hesvh.cn/Article/details/gpismrazf.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fehbvm.com/Article/details/grhtohzcm.sHtML

[S11] C：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gowssxapw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fehbvm.com/Article/details/gzaavgjmy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fehbvm.com/Article/details/gyeebimxa.sHtML

fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gupdiuuin.sHtML

[S12] C：写文件
来源：http://mobile.zdbjq.cn/Article/details/ggzqpoock.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fehbvm.com/Article/details/gxfwgjjnd.sHtML

[S13] C：宏定义
来源：http://www.share.hesvh.cn/Article/details/gmkkynlib.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.zdbjq.cn/Article/details/gamgypuxj.sHtML

[S14] C：枚举
来源：http://www.blog.hesvh.cn/Article/details/guuhobcya.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.hesvh.cn/Article/details/goqmnyvel.sHtML

[S15] C：类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gtfczjbeq.sHtML

(double) a / b
来源：http://blog.fehbvm.com/Article/details/gxcorgpho.sHtML

[S16] C：位操作置位
来源：http://m.share.hesvh.cn/Article/details/gcdcbhuca.sHtML

x |= (1 << 3);
来源：http://m.share.zdbjq.cn/Article/details/gcjwiizwp.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fehbvm.com/Article/details/gtobymgar.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fehbvm.com/Article/details/gdmkzqeed.sHtML

[S18] C：命令行参数
来源：http://mobile.zdbjq.cn/Article/details/gpftnunuc.sHtML

int main(int argc, char **argv)
来源：http://read.share.hesvh.cn/Article/details/geicvunin.sHtML

[S19] C：快速排序
来源：http://m.share.zdbjq.cn/Article/details/gyzkvucih.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/gherbznjz.sHtML

[S20] C：二分查找
来源：http://mobile.hesvh.cn/Article/details/glbxgsdtr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/gcrxiasua.sHtML

[S21] C：字符类别判断
来源：http://baike.zdbjq.cn/Article/details/gjfzutvcb.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.zdbjq.cn/Article/details/gphoxokjb.sHtML

[S22] C：字符串转数字
来源：http://m.share.fehbvm.com/Article/details/gvlyymvqj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fehbvm.com/Article/details/glaeytcwo.sHtML

[S23] C：随机数
来源：http://www.m.share.zdbjq.cn/Article/details/gbaweujox.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.hesvh.cn/Article/details/godvzfdpw.sHtML

[S24] C：获取本地时间
来源：http://blog.fehbvm.com/Article/details/gqczbqyia.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.hesvh.cn/Article/details/ggosjqrro.sHtML

[S25] C：内存拷贝
来源：http://mobile.fehbvm.com/Article/details/gqixrgonj.sHtML

memcpy(dst, src, n);
来源：http://blog.fehbvm.com/Article/details/gvupshyan.sHtML

[S26] C：内存清零
来源：http://read.share.hesvh.cn/Article/details/gajjzmysv.sHtML

memset(a, 0, sizeof a);
来源：http://3g.zdbjq.cn/Article/details/goiyjnrzk.sHtML

[S27] C：定义常量
来源：http://www.share.hesvh.cn/Article/details/gfotszgdz.sHtML

const double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/glifwpcwm.sHtML

[S28] C：静态变量
来源：http://wap.hesvh.cn/Article/details/gfanlircc.sHtML

static int counter = 0;
来源：http://read.share.zdbjq.cn/Article/details/gkfpxyhan.sHtML

[S29] C：变参函数
来源：http://www.blog.zdbjq.cn/Article/details/gxnhmorvn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.hesvh.cn/Article/details/gntryqiso.sHtML

[S30] C：头文件保护
来源：http://wap.fehbvm.com/Article/details/gnfstigvu.sHtML

#ifndef X_H
来源：http://read.share.fehbvm.com/Article/details/gbmzfonmw.sHtML

#define X_H
来源：http://read.share.hesvh.cn/Article/details/ghetpokww.sHtML

#endif
来源：http://m.share.fehbvm.com/Article/details/gogrxzilf.sHtML

[S31] C++：Hello World
来源：http://mobile.hesvh.cn/Article/details/gzcgsktws.sHtML

#include <iostream>
来源：http://mobile.zdbjq.cn/Article/details/gqcxfwywz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.hesvh.cn/Article/details/gozruywib.sHtML

[S32] C++：字符串
来源：http://mobile.zdbjq.cn/Article/details/gvtuqbopb.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fehbvm.com/Article/details/gshteryrb.sHtML

[S33] C++：vector 增删
来源：http://www.blog.zdbjq.cn/Article/details/gavqncbau.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fehbvm.com/Article/details/gehpbigig.sHtML

[S34] C++：遍历 vector
来源：http://baike.hesvh.cn/Article/details/gwzqfrngs.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.hesvh.cn/Article/details/gmbvyiukb.sHtML

[S35] C++：map
来源：http://m.share.zdbjq.cn/Article/details/gtwmvcdpi.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/guikrxdfa.sHtML

[S36] C++：unordered_map
来源：http://read.share.hesvh.cn/Article/details/gfyahbtem.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gvocdxzwa.sHtML

[S37] C++：set
来源：http://baike.fehbvm.com/Article/details/gdlsiskan.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fehbvm.com/Article/details/gpdkgntew.sHtML

[S38] C++：排序
来源：http://www.m.share.fehbvm.com/Article/details/gjgawzqii.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.hesvh.cn/Article/details/gvorlvcse.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fehbvm.com/Article/details/gpxteqlao.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.hesvh.cn/Article/details/gpkdgjwev.sHtML

[S40] C++：查找元素
来源：http://blog.hesvh.cn/Article/details/gsahbyeoq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.zdbjq.cn/Article/details/grdwxivab.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fehbvm.com/Article/details/gdutvliqg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.zdbjq.cn/Article/details/gulccglma.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fehbvm.com/Article/details/gtlppqtdk.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.hesvh.cn/Article/details/grrhecddo.sHtML

[S43] C++：智能指针
来源：http://www.blog.hesvh.cn/Article/details/gyneksnrq.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fehbvm.com/Article/details/grlafzwne.sHtML

[S44] C++：引用传参
来源：http://www.blog.zdbjq.cn/Article/details/gvbpnaehd.sHtML

void inc(int &x) { ++x; }
来源：http://blog.zdbjq.cn/Article/details/glaebvyjo.sHtML

[S45] C++：lambda
来源：http://www.share.fehbvm.com/Article/details/gnwcsilyu.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.hesvh.cn/Article/details/gsbrtfcqt.sHtML

[S46] C++：函数模板
来源：http://read.share.hesvh.cn/Article/details/gknwltzvf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.zdbjq.cn/Article/details/gflzujquy.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.zdbjq.cn/Article/details/gabthsedl.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fehbvm.com/Article/details/gibjqsshp.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gwszfflsb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.zdbjq.cn/Article/details/gheqfafph.sHtML


<!-- 参考信息 -->