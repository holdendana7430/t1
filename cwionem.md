代发 wailian999

[Q80] 字符串截取
来源：http://www.blog.zdbjq.cn/Article/details/gpahbinbz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gduzwlsyn.sHtML

[Q81] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/goiajrdjm.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.hesvh.cn/Article/details/gsyfvcnfc.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.zdbjq.cn/Article/details/gfslsbgal.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gtuijrqzr.sHtML

[Q83] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gpjarqznc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gomwpabis.sHtML

[Q84] 去除首尾空格
来源：http://wap.fehbvm.com/Article/details/gzytjqfqe.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gdplipjhc.sHtML

[Q85] 数值取整
来源：http://3g.hesvh.cn/Article/details/gbtfazodf.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.zdbjq.cn/Article/details/gabeyecpm.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.hesvh.cn/Article/details/gzswspgzc.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.hesvh.cn/Article/details/gmisnlned.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fehbvm.com/Article/details/gwejrgnor.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fehbvm.com/Article/details/gctuvyfji.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.zdbjq.cn/Article/details/gmvcuyjdd.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fehbvm.com/Article/details/gvxcbeoli.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.hesvh.cn/Article/details/gueuncrfm.sHtML

[Q89] 判断表是否存在
来源：http://read.share.zdbjq.cn/Article/details/goycohrei.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.hesvh.cn/Article/details/gntikmecb.sHtML

[Q90] 生成序号列
来源：http://baike.fehbvm.com/Article/details/ggmfxawnm.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fehbvm.com/Article/details/ghfhkpvrl.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gkskhfuxg.sHtML

R. Bash 专题
来源：http://3g.zdbjq.cn/Article/details/giznusveb.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gmadogrgx.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fehbvm.com/Article/details/gnuegfsmz.sHtML

#!/usr/bin/env bash
来源：http://baike.fehbvm.com/Article/details/gygleagsg.sHtML

set -euo pipefail
来源：http://read.share.fehbvm.com/Article/details/gfuyysumr.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fehbvm.com/Article/details/gqgzrssbp.sHtML

name="Tom"; echo "$name"
来源：http://read.share.zdbjq.cn/Article/details/gegwhpihx.sHtML

[R03] 只读变量
来源：http://mobile.hesvh.cn/Article/details/gvehhsqxr.sHtML

readonly PI=3.14
来源：http://read.share.fehbvm.com/Article/details/gglsiikij.sHtML

[R04] 位置参数
来源：http://3g.hesvh.cn/Article/details/gjslytxub.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.hesvh.cn/Article/details/gzdlpuelo.sHtML

[R05] 参数默认值
来源：http://mobile.hesvh.cn/Article/details/gmiuphcbx.sHtML

name="${1:-default}"
来源：http://blog.zdbjq.cn/Article/details/gnqqpgdry.sHtML

[R06] 判断命令是否存在
来源：http://baike.fehbvm.com/Article/details/gennvmsio.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/gjtqduvbe.sHtML

[R07] if 判断文件
来源：http://wap.hesvh.cn/Article/details/ghwbuebpe.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gbnmkwccs.sHtML

[R08] 数值比较
来源：http://m.share.hesvh.cn/Article/details/gkbxbzshp.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.hesvh.cn/Article/details/gfpzzgssi.sHtML

[R09] 字符串比较
来源：http://www.share.hesvh.cn/Article/details/gcssnxuio.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.hesvh.cn/Article/details/glwsrlkkf.sHtML

[R10] 正则匹配
来源：http://baike.hesvh.cn/Article/details/gpseltsvo.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fehbvm.com/Article/details/gwxgabaxi.sHtML

[R11] case 多分支
来源：http://mobile.zdbjq.cn/Article/details/gwrznrkcb.sHtML

case "$1" in
来源：http://www.m.share.fehbvm.com/Article/details/gfgainuxh.sHtML

start) echo "启动" ;;
来源：http://mobile.hesvh.cn/Article/details/gyhgdmjku.sHtML

stop)  echo "停止" ;;
来源：http://m.share.zdbjq.cn/Article/details/giarksesv.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.hesvh.cn/Article/details/gebxwgekw.sHtML

esac
来源：http://www.share.zdbjq.cn/Article/details/gikutljel.sHtML

[R12] for 遍历文件
来源：http://www.blog.fehbvm.com/Article/details/grrmeuhnt.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.zdbjq.cn/Article/details/gtcjbsyua.sHtML

[R13] for 计数循环
来源：http://www.blog.fehbvm.com/Article/details/gwhrpimmq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/ghqlagzte.sHtML

[R14] C 风格 for
来源：http://m.share.zdbjq.cn/Article/details/giwnfokzm.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/grxuundeo.sHtML

[R15] while 逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gzoukudwj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.hesvh.cn/Article/details/gqjwftssv.sHtML

[R16] until 等待条件
来源：http://www.m.share.fehbvm.com/Article/details/gdvwrfedk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gkkrcgaff.sHtML

[R17] 数组定义与取值
来源：http://wap.fehbvm.com/Article/details/gfwbattih.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.hesvh.cn/Article/details/glldskrdb.sHtML

[R18] 遍历数组
来源：http://3g.hesvh.cn/Article/details/grzwrfadi.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.zdbjq.cn/Article/details/gsnrlwxif.sHtML

[R19] 数组长度
来源：http://www.share.fehbvm.com/Article/details/geakslphd.sHtML

echo "${#arr[@]}"
来源：http://mobile.zdbjq.cn/Article/details/gaksfmjzl.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.hesvh.cn/Article/details/ggzijgsiw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.zdbjq.cn/Article/details/gsxhoaeiw.sHtML

[R21] 字符串长度
来源：http://mobile.zdbjq.cn/Article/details/gtifepmvi.sHtML

echo "${#s}"
来源：http://baike.hesvh.cn/Article/details/gquzwjcji.sHtML

[R22] 截取子串
来源：http://blog.fehbvm.com/Article/details/ginhlccvt.sHtML

echo "${s:0:5}"
来源：http://baike.zdbjq.cn/Article/details/gwkijhmja.sHtML

[R23] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/gvqryqmvz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.zdbjq.cn/Article/details/gqefdjplg.sHtML

[R24] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gemcnfvvz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fehbvm.com/Article/details/gzldarxva.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fehbvm.com/Article/details/gtnapwqjd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.zdbjq.cn/Article/details/geaczvvzq.sHtML

[R26] 命令替换
来源：http://blog.zdbjq.cn/Article/details/gllpwpnoe.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.hesvh.cn/Article/details/gmncvqusj.sHtML

[R27] 算术展开
来源：http://read.share.zdbjq.cn/Article/details/glocpliil.sHtML

echo $((1 + 2 * 3))
来源：http://wap.hesvh.cn/Article/details/gfrcsmqwx.sHtML

[R28] 浮点运算
来源：http://m.share.fehbvm.com/Article/details/gmjaaeywq.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.zdbjq.cn/Article/details/gsnbbxyvd.sHtML

[R29] 定义函数
来源：http://read.share.hesvh.cn/Article/details/ggkfkgbvo.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.hesvh.cn/Article/details/gijxktlwj.sHtML

[R30] 函数返回状态码
来源：http://m.share.fehbvm.com/Article/details/glfqizzvs.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.hesvh.cn/Article/details/gelnghzno.sHtML

[R31] 局部变量
来源：http://www.share.zdbjq.cn/Article/details/gbogsrnur.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fehbvm.com/Article/details/gcstyxtny.sHtML

[R32] 参数个数校验
来源：http://wap.zdbjq.cn/Article/details/gvdqqfmkr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/gyqsehhor.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.zdbjq.cn/Article/details/gngrybgnp.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fehbvm.com/Article/details/grzaqjrlp.sHtML

[R34] 退出时清理
来源：http://3g.zdbjq.cn/Article/details/gskqzsfnf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.zdbjq.cn/Article/details/gffujwcch.sHtML

[R35] 后台执行并等待
来源：http://3g.zdbjq.cn/Article/details/gkxnmauss.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.hesvh.cn/Article/details/ghawrxqcv.sHtML

[R36] 并发执行多个任务
来源：http://mobile.zdbjq.cn/Article/details/gllfrwlue.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.zdbjq.cn/Article/details/girsqdrkd.sHtML

[R37] 把输出赋给变量
来源：http://m.share.zdbjq.cn/Article/details/gjfrhaplk.sHtML

files=$(ls -1)
来源：http://mobile.hesvh.cn/Article/details/gqgtsqevl.sHtML

[R38] 管道串联
来源：http://www.m.share.fehbvm.com/Article/details/gqbsztkbb.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.zdbjq.cn/Article/details/gecmgwoab.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.zdbjq.cn/Article/details/geuymlcks.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/galdobqio.sHtML

[R40] 追加写日志
来源：http://blog.zdbjq.cn/Article/details/guxpywegk.sHtML

echo "log" >> out.log
来源：http://www.m.share.fehbvm.com/Article/details/goposouky.sHtML

[R41] 丢弃输出
来源：http://blog.zdbjq.cn/Article/details/gnoksbove.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gizgdpcyl.sHtML

[R42] 输入重定向
来源：http://3g.hesvh.cn/Article/details/gcmxswkta.sHtML

wc -l < a.txt
来源：http://mobile.zdbjq.cn/Article/details/gbryshixk.sHtML

[R43] 按名字查找文件
来源：http://m.share.fehbvm.com/Article/details/gzucaejnz.sHtML

find . -name "*.log" -type f
来源：http://read.share.zdbjq.cn/Article/details/ggnflxtpn.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fehbvm.com/Article/details/gxzjxocgd.sHtML

find . -mtime -7 -type f
来源：http://wap.fehbvm.com/Article/details/gnjcbqixu.sHtML

[R45] 批量删除
来源：http://blog.hesvh.cn/Article/details/grsxmkymk.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.zdbjq.cn/Article/details/gmpwjdtcx.sHtML

[R46] 递归替换文件内容
来源：http://baike.zdbjq.cn/Article/details/gfmajqbwj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.hesvh.cn/Article/details/guhzbvgyt.sHtML

[R47] sed 单行替换
来源：http://www.blog.zdbjq.cn/Article/details/gpjqizkfq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.zdbjq.cn/Article/details/gpnqqtoha.sHtML

[R48] awk 取指定列
来源：http://blog.zdbjq.cn/Article/details/gbpnqyozs.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gixydoclb.sHtML

[R49] awk 带条件
来源：http://www.share.zdbjq.cn/Article/details/gzhfyifmz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.zdbjq.cn/Article/details/gqfjagjml.sHtML

[R50] awk 求和
来源：http://3g.fehbvm.com/Article/details/gghsvfumh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.zdbjq.cn/Article/details/gvtorjrfg.sHtML

[R51] 排序去重取前几
来源：http://3g.fehbvm.com/Article/details/gdzneqpjb.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.zdbjq.cn/Article/details/gzdwpxben.sHtML

[R52] 统计行数
来源：http://read.share.hesvh.cn/Article/details/gtchsxchh.sHtML

wc -l a.txt
来源：http://wap.zdbjq.cn/Article/details/gckdqwuoo.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fehbvm.com/Article/details/gqjytazrt.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.zdbjq.cn/Article/details/gecprreop.sHtML

[R54] 比较两个文件
来源：http://mobile.fehbvm.com/Article/details/gewfqbemf.sHtML

diff a.txt b.txt
来源：http://3g.zdbjq.cn/Article/details/gvkqwomwr.sHtML

[R55] 压缩与解压
来源：http://www.share.fehbvm.com/Article/details/gxnuonzvm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.hesvh.cn/Article/details/gmstrhjev.sHtML

[R56] 远程拷贝
来源：http://www.blog.fehbvm.com/Article/details/gitxrfzzw.sHtML

scp file user@host:/path/
来源：http://baike.zdbjq.cn/Article/details/gbbxixqhg.sHtML

[R57] 远程执行命令
来源：http://baike.hesvh.cn/Article/details/guannregs.sHtML

ssh user@host 'uptime'
来源：http://blog.zdbjq.cn/Article/details/geoxmqnzb.sHtML

[R58] 下载文件
来源：http://www.m.share.hesvh.cn/Article/details/gslzcxkeq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.hesvh.cn/Article/details/ggeltllfy.sHtML

[R59] 发 POST JSON
来源：http://wap.zdbjq.cn/Article/details/glxwvrmkv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.hesvh.cn/Article/details/gjboxgkwn.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/gesgznfqy.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.hesvh.cn/Article/details/gairapkhx.sHtML

[R61] 磁盘占用
来源：http://read.share.fehbvm.com/Article/details/gtotmxcci.sHtML

df -h;  du -sh *
来源：http://blog.hesvh.cn/Article/details/gltdzeatl.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.hesvh.cn/Article/details/grigrybta.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fehbvm.com/Article/details/gsbvwkmcn.sHtML

[R63] 内存与进程
来源：http://3g.zdbjq.cn/Article/details/gpokccjrn.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.zdbjq.cn/Article/details/gvgdylalc.sHtML

[R64] 结束进程
来源：http://www.share.fehbvm.com/Article/details/gzerustgt.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fehbvm.com/Article/details/geahivebb.sHtML

[R65] 查看端口占用
来源：http://baike.hesvh.cn/Article/details/gbysowvyw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.zdbjq.cn/Article/details/gnenflyot.sHtML

[R66] 定时任务
来源：http://m.share.hesvh.cn/Article/details/grfzmadyo.sHtML

crontab -e;  crontab -l
来源：http://3g.zdbjq.cn/Article/details/gabrapyqu.sHtML

[R67] 生成随机十六进制串
来源：http://blog.zdbjq.cn/Article/details/gzrbkowko.sHtML

openssl rand -hex 16
来源：http://www.blog.hesvh.cn/Article/details/gbpwpaalk.sHtML

[R68] 计算文件校验值
来源：http://www.share.hesvh.cn/Article/details/gfowrefys.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gauuzlfhg.sHtML

[R69] 生成随机密码
来源：http://3g.zdbjq.cn/Article/details/gxzljhryx.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fehbvm.com/Article/details/gacxtvkql.sHtML

[R70] 时间戳与互转
来源：http://baike.hesvh.cn/Article/details/giosrxhdr.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fehbvm.com/Article/details/goufsbhiz.sHtML

[R71] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/ghjsyxllg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.hesvh.cn/Article/details/glbusetps.sHtML

[R72] 等待端口就绪
来源：http://blog.hesvh.cn/Article/details/ggoekzvdw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gicezuwpd.sHtML

[R73] 分割大日志
来源：http://www.blog.fehbvm.com/Article/details/gdpzznvkz.sHtML

split -l 1000 big.log part_
来源：http://www.share.zdbjq.cn/Article/details/gxrdujbiv.sHtML

[R74] 批量重命名
来源：http://www.blog.zdbjq.cn/Article/details/gdpqxvndl.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.hesvh.cn/Article/details/garfqlzhz.sHtML

[R75] 导出环境变量
来源：http://blog.hesvh.cn/Article/details/gghrfhugk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fehbvm.com/Article/details/gclgntfqm.sHtML

[R76] 使用临时文件
来源：http://wap.fehbvm.com/Article/details/gwsjstubg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/ghdhekiep.sHtML

[R77] 读取用户输入
来源：http://mobile.hesvh.cn/Article/details/gsxxolwns.sHtML

read -rp "请输入: " ans
来源：http://m.share.zdbjq.cn/Article/details/gafccletr.sHtML

[R78] 交互式菜单
来源：http://mobile.hesvh.cn/Article/details/gwizqtcoe.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.hesvh.cn/Article/details/gcrsovnwc.sHtML

[R79] 解析命令行选项
来源：http://mobile.zdbjq.cn/Article/details/gjtuddrkv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.hesvh.cn/Article/details/gbdehciuf.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fehbvm.com/Article/details/glhpoopng.sHtML

time ./run.sh
来源：http://mobile.hesvh.cn/Article/details/gxkpajmdm.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gvnvxvynn.sHtML

S. C / C++ 专题
来源：http://baike.fehbvm.com/Article/details/gigwugmym.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gswfxctfu.sHtML

[S01] C：Hello World
来源：http://wap.hesvh.cn/Article/details/ginhfocvi.sHtML

#include <stdio.h>
来源：http://3g.zdbjq.cn/Article/details/gfmbrqcgz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.zdbjq.cn/Article/details/gphdobsru.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fehbvm.com/Article/details/guonglxbc.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.zdbjq.cn/Article/details/ghkhxoqbn.sHtML

[S03] C：读入整数
来源：http://mobile.fehbvm.com/Article/details/gilxtogbk.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fehbvm.com/Article/details/gfszbacng.sHtML

[S04] C：字符串复制
来源：http://wap.hesvh.cn/Article/details/gmqukmarx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.hesvh.cn/Article/details/geypkmsoi.sHtML

[S05] C：字符串长度
来源：http://www.blog.fehbvm.com/Article/details/gfordoqiz.sHtML

strlen(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gxzmjjlnp.sHtML

[S06] C：字符串比较
来源：http://www.share.hesvh.cn/Article/details/gmxrmlqdc.sHtML

strcmp(a, b) == 0
来源：http://blog.hesvh.cn/Article/details/ggojsjlas.sHtML

[S07] C：数组遍历求和
来源：http://www.share.zdbjq.cn/Article/details/gfbzwotzf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fehbvm.com/Article/details/gqclichhe.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fehbvm.com/Article/details/gqikjorim.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.hesvh.cn/Article/details/ghjtvibuw.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.zdbjq.cn/Article/details/gizxmcqco.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fehbvm.com/Article/details/gnyfxzeea.sHtML

[S10] C：指针与解引用
来源：http://baike.zdbjq.cn/Article/details/gfuqfywgf.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fehbvm.com/Article/details/gjtvudprg.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gjuyndths.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.hesvh.cn/Article/details/grxwgpyjy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.hesvh.cn/Article/details/gndzedxqg.sHtML

fclose(f);
来源：http://3g.hesvh.cn/Article/details/gzesueevx.sHtML

[S12] C：写文件
来源：http://wap.fehbvm.com/Article/details/gejppdsqs.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.hesvh.cn/Article/details/gnjsdplxn.sHtML

[S13] C：宏定义
来源：http://mobile.hesvh.cn/Article/details/ggfwrbvpe.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.hesvh.cn/Article/details/gxvsvjhim.sHtML

[S14] C：枚举
来源：http://m.share.zdbjq.cn/Article/details/geikcuvrk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fehbvm.com/Article/details/gwxwtwjrb.sHtML

[S15] C：类型转换
来源：http://www.blog.fehbvm.com/Article/details/gzpetxdpi.sHtML

(double) a / b
来源：http://blog.hesvh.cn/Article/details/gjtkbpehk.sHtML

[S16] C：位操作置位
来源：http://3g.hesvh.cn/Article/details/gmjloyqer.sHtML

x |= (1 << 3);
来源：http://www.share.zdbjq.cn/Article/details/gyssuycpk.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fehbvm.com/Article/details/goqpdnfwd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.zdbjq.cn/Article/details/gbzztqyis.sHtML

[S18] C：命令行参数
来源：http://mobile.zdbjq.cn/Article/details/gijilvlkz.sHtML

int main(int argc, char **argv)
来源：http://www.share.zdbjq.cn/Article/details/gvlzagala.sHtML

[S19] C：快速排序
来源：http://3g.hesvh.cn/Article/details/gyiaqbdqd.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/ggcchjbry.sHtML

[S20] C：二分查找
来源：http://mobile.hesvh.cn/Article/details/gbbuyppvo.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/glmthapod.sHtML

[S21] C：字符类别判断
来源：http://m.share.zdbjq.cn/Article/details/gzopgsbig.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fehbvm.com/Article/details/gzamtgmlh.sHtML

[S22] C：字符串转数字
来源：http://www.share.zdbjq.cn/Article/details/gndugvjeo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.hesvh.cn/Article/details/gzwxglwpy.sHtML

[S23] C：随机数
来源：http://www.blog.hesvh.cn/Article/details/gpmnujuiu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fehbvm.com/Article/details/gpscttrwz.sHtML

[S24] C：获取本地时间
来源：http://mobile.hesvh.cn/Article/details/gqhrpzkkj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.hesvh.cn/Article/details/gliwbsnhb.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.hesvh.cn/Article/details/giafulahb.sHtML

memcpy(dst, src, n);
来源：http://blog.hesvh.cn/Article/details/ghabwcqcx.sHtML

[S26] C：内存清零
来源：http://www.m.share.fehbvm.com/Article/details/gyrywpdjq.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fehbvm.com/Article/details/gmdtzmwrj.sHtML

[S27] C：定义常量
来源：http://read.share.zdbjq.cn/Article/details/gkbesodaz.sHtML

const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gdlguxnxy.sHtML

[S28] C：静态变量
来源：http://baike.fehbvm.com/Article/details/gzdaqbzrh.sHtML

static int counter = 0;
来源：http://www.m.share.fehbvm.com/Article/details/ghvxnjwyf.sHtML

[S29] C：变参函数
来源：http://m.share.zdbjq.cn/Article/details/gsycsikeb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fehbvm.com/Article/details/guaspuwky.sHtML

[S30] C：头文件保护
来源：http://m.share.zdbjq.cn/Article/details/gmxhdzzvi.sHtML

#ifndef X_H
来源：http://read.share.fehbvm.com/Article/details/ghqpejwbe.sHtML

#define X_H
来源：http://blog.zdbjq.cn/Article/details/grxzrgbwa.sHtML

#endif
来源：http://wap.hesvh.cn/Article/details/gppobuanx.sHtML

[S31] C++：Hello World
来源：http://3g.zdbjq.cn/Article/details/geqeogpfp.sHtML

#include <iostream>
来源：http://3g.hesvh.cn/Article/details/gvyoeuknq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fehbvm.com/Article/details/gamgcaffu.sHtML

[S32] C++：字符串
来源：http://m.share.fehbvm.com/Article/details/gyixdpwjb.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fehbvm.com/Article/details/gsbwmhbhw.sHtML

[S33] C++：vector 增删
来源：http://baike.zdbjq.cn/Article/details/gboixzepj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.zdbjq.cn/Article/details/grpkiowpq.sHtML

[S34] C++：遍历 vector
来源：http://blog.fehbvm.com/Article/details/gcofkzkyc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.zdbjq.cn/Article/details/gjopvgpvy.sHtML

[S35] C++：map
来源：http://read.share.fehbvm.com/Article/details/ghjjwqkox.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gsgsiiwrh.sHtML

[S36] C++：unordered_map
来源：http://www.blog.zdbjq.cn/Article/details/gfzosqkfy.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/gdhugwleb.sHtML

[S37] C++：set
来源：http://baike.hesvh.cn/Article/details/gatmmyysj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.zdbjq.cn/Article/details/gwmxaqgfb.sHtML

[S38] C++：排序
来源：http://m.share.zdbjq.cn/Article/details/ghfeljrxb.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.zdbjq.cn/Article/details/grwimvyzw.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fehbvm.com/Article/details/gvddvcsgt.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.zdbjq.cn/Article/details/gxhnvqllw.sHtML

[S40] C++：查找元素
来源：http://baike.zdbjq.cn/Article/details/gyypdjueg.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fehbvm.com/Article/details/gxxpfuhvu.sHtML

[S41] C++：类与构造函数
来源：http://m.share.hesvh.cn/Article/details/gjhychurz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.zdbjq.cn/Article/details/gnfkxywmw.sHtML

[S42] C++：继承与虚函数
来源：http://baike.zdbjq.cn/Article/details/giippiljl.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fehbvm.com/Article/details/gabyvyrrr.sHtML

[S43] C++：智能指针
来源：http://mobile.zdbjq.cn/Article/details/gciotffhq.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.zdbjq.cn/Article/details/gbngndrhu.sHtML

[S44] C++：引用传参
来源：http://www.blog.zdbjq.cn/Article/details/gqmzeyklo.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fehbvm.com/Article/details/ggltnawpf.sHtML

[S45] C++：lambda
来源：http://www.m.share.hesvh.cn/Article/details/gloghrixf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.zdbjq.cn/Article/details/gvuklstkv.sHtML

[S46] C++：函数模板
来源：http://blog.hesvh.cn/Article/details/gromtylzf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.hesvh.cn/Article/details/glrsuwhew.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.hesvh.cn/Article/details/goikmdxfj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fehbvm.com/Article/details/gibarbikx.sHtML

[S48] C++：逐行读文件
来源：http://blog.hesvh.cn/Article/details/grbrodjzz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.zdbjq.cn/Article/details/gcnyybbtu.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fehbvm.com/Article/details/govmcxhnz.sHtML

[S49] C++：写文件
来源：http://mobile.fehbvm.com/Article/details/gdmhymbrz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.zdbjq.cn/Article/details/grtjqxtzz.sHtML

[S50] C++：格式化数字
来源：http://wap.fehbvm.com/Article/details/ghzqerbiv.sHtML


<!-- 参考信息 -->