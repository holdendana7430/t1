代发 wailian999

[Q80] 字符串截取
来源：http://www.share.fehbvm.com/Article/details/gidtnezuw.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.zdbjq.cn/Article/details/ghwtwaioo.sHtML

[Q81] 字符串替换
来源：http://3g.fehbvm.com/Article/details/gnldbrrxm.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fehbvm.com/Article/details/gmaeoxqix.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fehbvm.com/Article/details/gqpptwklc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gyhaepmxq.sHtML

[Q83] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gcgxuvayw.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gbujrksgi.sHtML

[Q84] 去除首尾空格
来源：http://3g.fehbvm.com/Article/details/gvusarpfa.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gykwbegds.sHtML

[Q85] 数值取整
来源：http://3g.fehbvm.com/Article/details/gukhomjnm.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.zdbjq.cn/Article/details/gwfxjkdjd.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.hesvh.cn/Article/details/ggdozukji.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.zdbjq.cn/Article/details/gvktqaejt.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.zdbjq.cn/Article/details/gsbwhqcxs.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fehbvm.com/Article/details/ggzejbnde.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.hesvh.cn/Article/details/gdhneeqmp.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fehbvm.com/Article/details/ghjzpvgfg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.zdbjq.cn/Article/details/gflzzprrx.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gnejaegxw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fehbvm.com/Article/details/gyhpukhya.sHtML

[Q90] 生成序号列
来源：http://3g.hesvh.cn/Article/details/gnubkhgbh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.hesvh.cn/Article/details/gopmkgbjr.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gkoojnqic.sHtML

R. Bash 专题
来源：http://baike.zdbjq.cn/Article/details/gocudkgwq.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gdxtleuwv.sHtML

[R01] shebang 与严格模式
来源：http://baike.fehbvm.com/Article/details/gdwljfcyw.sHtML

#!/usr/bin/env bash
来源：http://www.blog.hesvh.cn/Article/details/gycicbfws.sHtML

set -euo pipefail
来源：http://3g.hesvh.cn/Article/details/gorkpskdg.sHtML

[R02] 变量赋值与使用
来源：http://mobile.hesvh.cn/Article/details/gppcfwmpq.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.zdbjq.cn/Article/details/ggxvesofp.sHtML

[R03] 只读变量
来源：http://blog.zdbjq.cn/Article/details/gufqevhqr.sHtML

readonly PI=3.14
来源：http://m.share.zdbjq.cn/Article/details/gtttpaexh.sHtML

[R04] 位置参数
来源：http://wap.hesvh.cn/Article/details/gbfkyiulz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.zdbjq.cn/Article/details/giphtgepj.sHtML

[R05] 参数默认值
来源：http://wap.fehbvm.com/Article/details/gvqjhfgmz.sHtML

name="${1:-default}"
来源：http://read.share.fehbvm.com/Article/details/gzreadbjp.sHtML

[R06] 判断命令是否存在
来源：http://3g.zdbjq.cn/Article/details/guswprvtn.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/gamjbwsnu.sHtML

[R07] if 判断文件
来源：http://mobile.zdbjq.cn/Article/details/gxmfmklvt.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fehbvm.com/Article/details/gmcwqbboe.sHtML

[R08] 数值比较
来源：http://m.share.fehbvm.com/Article/details/gfmkamioa.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.hesvh.cn/Article/details/gggpwekxd.sHtML

[R09] 字符串比较
来源：http://m.share.hesvh.cn/Article/details/ggkqquflp.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.zdbjq.cn/Article/details/gqqdrdxfe.sHtML

[R10] 正则匹配
来源：http://www.blog.hesvh.cn/Article/details/gsfcqauix.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fehbvm.com/Article/details/gasjpczhz.sHtML

[R11] case 多分支
来源：http://mobile.zdbjq.cn/Article/details/guanjttji.sHtML

case "$1" in
来源：http://www.share.hesvh.cn/Article/details/gsnwjdbqc.sHtML

start) echo "启动" ;;
来源：http://3g.fehbvm.com/Article/details/gjvtpdzes.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gzrwcwrbe.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.zdbjq.cn/Article/details/gytspkicv.sHtML

esac
来源：http://baike.zdbjq.cn/Article/details/gejwtbpht.sHtML

[R12] for 遍历文件
来源：http://m.share.hesvh.cn/Article/details/gwbhugxvs.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fehbvm.com/Article/details/gdrykjjko.sHtML

[R13] for 计数循环
来源：http://www.share.fehbvm.com/Article/details/gifzgiler.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/gaftatcrz.sHtML

[R14] C 风格 for
来源：http://www.share.zdbjq.cn/Article/details/geuruznak.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gvpjjbyae.sHtML

[R15] while 逐行读文件
来源：http://3g.zdbjq.cn/Article/details/guezobtug.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.zdbjq.cn/Article/details/gedihteul.sHtML

[R16] until 等待条件
来源：http://3g.hesvh.cn/Article/details/gemwiqdcf.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gtwjngjih.sHtML

[R17] 数组定义与取值
来源：http://wap.fehbvm.com/Article/details/gqydlhhpi.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fehbvm.com/Article/details/gpxaatwoh.sHtML

[R18] 遍历数组
来源：http://blog.zdbjq.cn/Article/details/gpewbxlsr.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.hesvh.cn/Article/details/gecqwwbpz.sHtML

[R19] 数组长度
来源：http://3g.hesvh.cn/Article/details/gytdckwxn.sHtML

echo "${#arr[@]}"
来源：http://m.share.fehbvm.com/Article/details/gbvxbojtr.sHtML

[R20] 关联数组（字典）
来源：http://www.share.hesvh.cn/Article/details/gzfdfgrvy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.hesvh.cn/Article/details/gotnjvqqu.sHtML

[R21] 字符串长度
来源：http://mobile.fehbvm.com/Article/details/ggllhxzlg.sHtML

echo "${#s}"
来源：http://blog.zdbjq.cn/Article/details/gleqpidyq.sHtML

[R22] 截取子串
来源：http://mobile.fehbvm.com/Article/details/ghrqbelst.sHtML

echo "${s:0:5}"
来源：http://blog.zdbjq.cn/Article/details/gjrmdvapk.sHtML

[R23] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/gwhjicksp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.zdbjq.cn/Article/details/grjaflthc.sHtML

[R24] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/gopiptxvw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fehbvm.com/Article/details/gcnsvziqc.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.zdbjq.cn/Article/details/gdkkzygnc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fehbvm.com/Article/details/gbeapboda.sHtML

[R26] 命令替换
来源：http://www.share.fehbvm.com/Article/details/gcyxbkrik.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.zdbjq.cn/Article/details/gslousjzw.sHtML

[R27] 算术展开
来源：http://www.share.hesvh.cn/Article/details/gggffjgoi.sHtML

echo $((1 + 2 * 3))
来源：http://wap.zdbjq.cn/Article/details/gusdgkwek.sHtML

[R28] 浮点运算
来源：http://baike.hesvh.cn/Article/details/gtzfdgdpn.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.zdbjq.cn/Article/details/gsyeapymn.sHtML

[R29] 定义函数
来源：http://mobile.fehbvm.com/Article/details/gwqtropko.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.zdbjq.cn/Article/details/gwgsbywdx.sHtML

[R30] 函数返回状态码
来源：http://blog.hesvh.cn/Article/details/gzahjdqun.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fehbvm.com/Article/details/ghdlftuss.sHtML

[R31] 局部变量
来源：http://3g.hesvh.cn/Article/details/gdoaiggqx.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fehbvm.com/Article/details/gdnoquphr.sHtML

[R32] 参数个数校验
来源：http://baike.zdbjq.cn/Article/details/gnhzbeqct.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/ghottphbx.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.hesvh.cn/Article/details/gavkqwfum.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.hesvh.cn/Article/details/gohbmcpip.sHtML

[R34] 退出时清理
来源：http://baike.fehbvm.com/Article/details/gvegkpnrb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gthkxkxkj.sHtML

[R35] 后台执行并等待
来源：http://m.share.hesvh.cn/Article/details/giavfbiqy.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.hesvh.cn/Article/details/gdhxytfyn.sHtML

[R36] 并发执行多个任务
来源：http://m.share.hesvh.cn/Article/details/gehogtzgj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.zdbjq.cn/Article/details/gbibxwnju.sHtML

[R37] 把输出赋给变量
来源：http://www.share.zdbjq.cn/Article/details/gxbrzhccd.sHtML

files=$(ls -1)
来源：http://www.share.hesvh.cn/Article/details/ghiniywkp.sHtML

[R38] 管道串联
来源：http://m.share.hesvh.cn/Article/details/gtetylwkc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fehbvm.com/Article/details/gfyahkmbx.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.hesvh.cn/Article/details/gczblfxgx.sHtML

cmd > out.log 2>&1
来源：http://wap.hesvh.cn/Article/details/gpbntvnar.sHtML

[R40] 追加写日志
来源：http://baike.hesvh.cn/Article/details/gkpybfibq.sHtML

echo "log" >> out.log
来源：http://www.m.share.fehbvm.com/Article/details/guhmuxwaz.sHtML

[R41] 丢弃输出
来源：http://3g.hesvh.cn/Article/details/gftmndmnp.sHtML

cmd >/dev/null 2>&1
来源：http://3g.hesvh.cn/Article/details/gccctdstc.sHtML

[R42] 输入重定向
来源：http://wap.zdbjq.cn/Article/details/gmtniqupt.sHtML

wc -l < a.txt
来源：http://3g.fehbvm.com/Article/details/gwnniaczc.sHtML

[R43] 按名字查找文件
来源：http://read.share.hesvh.cn/Article/details/gdnrmrmaa.sHtML

find . -name "*.log" -type f
来源：http://wap.fehbvm.com/Article/details/gszowvrpa.sHtML

[R44] 按修改时间查找
来源：http://wap.zdbjq.cn/Article/details/gyooymgwv.sHtML

find . -mtime -7 -type f
来源：http://www.blog.hesvh.cn/Article/details/gogkqvgse.sHtML

[R45] 批量删除
来源：http://3g.hesvh.cn/Article/details/gdnsgarjq.sHtML

find . -name "*.tmp" -delete
来源：http://baike.zdbjq.cn/Article/details/ghijkzhwh.sHtML

[R46] 递归替换文件内容
来源：http://wap.fehbvm.com/Article/details/gngglbpnm.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fehbvm.com/Article/details/gbdjjycko.sHtML

[R47] sed 单行替换
来源：http://wap.fehbvm.com/Article/details/gnoghcjvn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.zdbjq.cn/Article/details/gxikmbrgx.sHtML

[R48] awk 取指定列
来源：http://read.share.fehbvm.com/Article/details/geeymblmo.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gkyrvdxud.sHtML

[R49] awk 带条件
来源：http://3g.hesvh.cn/Article/details/gwckytrva.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.zdbjq.cn/Article/details/gywiqfulc.sHtML

[R50] awk 求和
来源：http://m.share.hesvh.cn/Article/details/gjxxhmnhs.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.hesvh.cn/Article/details/gkiawtobn.sHtML

[R51] 排序去重取前几
来源：http://wap.fehbvm.com/Article/details/geuvysrod.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fehbvm.com/Article/details/grjomchuk.sHtML

[R52] 统计行数
来源：http://wap.fehbvm.com/Article/details/glzdyirjq.sHtML

wc -l a.txt
来源：http://3g.fehbvm.com/Article/details/glkizrokq.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fehbvm.com/Article/details/gxzllmsrj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.hesvh.cn/Article/details/gmjblzntc.sHtML

[R54] 比较两个文件
来源：http://mobile.zdbjq.cn/Article/details/gbeepseeo.sHtML

diff a.txt b.txt
来源：http://www.share.fehbvm.com/Article/details/gkembydlg.sHtML

[R55] 压缩与解压
来源：http://read.share.zdbjq.cn/Article/details/ghlvkqmyu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.zdbjq.cn/Article/details/gcincjwsj.sHtML

[R56] 远程拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/glnjbnzwi.sHtML

scp file user@host:/path/
来源：http://www.share.fehbvm.com/Article/details/gzmdiyndn.sHtML

[R57] 远程执行命令
来源：http://www.blog.fehbvm.com/Article/details/galelehcv.sHtML

ssh user@host 'uptime'
来源：http://www.blog.hesvh.cn/Article/details/gxgvytimp.sHtML

[R58] 下载文件
来源：http://www.m.share.zdbjq.cn/Article/details/gdhczrspa.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.hesvh.cn/Article/details/glipoywlw.sHtML

[R59] 发 POST JSON
来源：http://3g.hesvh.cn/Article/details/gjynyrzod.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fehbvm.com/Article/details/ghismgspv.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/gogbmfquz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.zdbjq.cn/Article/details/glmgtwhsd.sHtML

[R61] 磁盘占用
来源：http://3g.fehbvm.com/Article/details/gfwgitxyj.sHtML

df -h;  du -sh *
来源：http://blog.hesvh.cn/Article/details/gwszrnadb.sHtML

[R62] 找最占空间的文件
来源：http://baike.zdbjq.cn/Article/details/giltyucwb.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.zdbjq.cn/Article/details/gkrqveohn.sHtML

[R63] 内存与进程
来源：http://3g.hesvh.cn/Article/details/ggiwxnjbe.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.hesvh.cn/Article/details/gazmeeihi.sHtML

[R64] 结束进程
来源：http://m.share.zdbjq.cn/Article/details/ghciholtd.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.hesvh.cn/Article/details/gpqjbirwj.sHtML

[R65] 查看端口占用
来源：http://read.share.fehbvm.com/Article/details/gprnqlfkh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.zdbjq.cn/Article/details/gwociwhdo.sHtML

[R66] 定时任务
来源：http://mobile.fehbvm.com/Article/details/gyynctjkg.sHtML

crontab -e;  crontab -l
来源：http://baike.fehbvm.com/Article/details/gynimpxao.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.hesvh.cn/Article/details/gphanrwzy.sHtML

openssl rand -hex 16
来源：http://mobile.hesvh.cn/Article/details/ghsefvupj.sHtML

[R68] 计算文件校验值
来源：http://m.share.zdbjq.cn/Article/details/gaeflkact.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fehbvm.com/Article/details/gkkvbadlv.sHtML

[R69] 生成随机密码
来源：http://m.share.hesvh.cn/Article/details/gsgeuhmun.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fehbvm.com/Article/details/gvzzmdfvd.sHtML

[R70] 时间戳与互转
来源：http://baike.fehbvm.com/Article/details/gzultqsof.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.zdbjq.cn/Article/details/gjowutknq.sHtML

[R71] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gowsgmgzz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fehbvm.com/Article/details/gxwhkpvjt.sHtML

[R72] 等待端口就绪
来源：http://mobile.zdbjq.cn/Article/details/gblbnqtbp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gyppwhtvp.sHtML

[R73] 分割大日志
来源：http://read.share.fehbvm.com/Article/details/gkblllmjx.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fehbvm.com/Article/details/gysynxhvy.sHtML

[R74] 批量重命名
来源：http://3g.fehbvm.com/Article/details/gorsgdfhz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.hesvh.cn/Article/details/glsguizlg.sHtML

[R75] 导出环境变量
来源：http://3g.zdbjq.cn/Article/details/gqzgkrzch.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.zdbjq.cn/Article/details/giapqrjmr.sHtML

[R76] 使用临时文件
来源：http://baike.zdbjq.cn/Article/details/gzabaszdr.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gxoltnatc.sHtML

[R77] 读取用户输入
来源：http://wap.hesvh.cn/Article/details/gkyyubfkz.sHtML

read -rp "请输入: " ans
来源：http://www.share.fehbvm.com/Article/details/guqscbbpe.sHtML

[R78] 交互式菜单
来源：http://mobile.fehbvm.com/Article/details/gvteruizf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fehbvm.com/Article/details/gaflqfuyf.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.hesvh.cn/Article/details/gpcbidzmw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fehbvm.com/Article/details/grredpdtp.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fehbvm.com/Article/details/gqqcwfztn.sHtML

time ./run.sh
来源：http://3g.fehbvm.com/Article/details/gzxaecmsb.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gevbghrsr.sHtML

S. C / C++ 专题
来源：http://www.share.hesvh.cn/Article/details/gbagankvj.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gyydltrrz.sHtML

[S01] C：Hello World
来源：http://wap.zdbjq.cn/Article/details/gktktqvlp.sHtML

#include <stdio.h>
来源：http://m.share.zdbjq.cn/Article/details/gprggwsde.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.zdbjq.cn/Article/details/glwfqvgli.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fehbvm.com/Article/details/ghjatsmfd.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.hesvh.cn/Article/details/gjrcugwkt.sHtML

[S03] C：读入整数
来源：http://3g.zdbjq.cn/Article/details/gjxehfrtz.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fehbvm.com/Article/details/gtyblqalc.sHtML

[S04] C：字符串复制
来源：http://www.m.share.zdbjq.cn/Article/details/gveyilnor.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gsfryqfbz.sHtML

[S05] C：字符串长度
来源：http://blog.zdbjq.cn/Article/details/gcavnpnsj.sHtML

strlen(s)
来源：http://www.m.share.zdbjq.cn/Article/details/ggyhlzpqc.sHtML

[S06] C：字符串比较
来源：http://blog.fehbvm.com/Article/details/grmtuohfa.sHtML

strcmp(a, b) == 0
来源：http://www.blog.hesvh.cn/Article/details/gumppqonf.sHtML

[S07] C：数组遍历求和
来源：http://mobile.zdbjq.cn/Article/details/goflbqiln.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.zdbjq.cn/Article/details/glfrkynvu.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.zdbjq.cn/Article/details/gsvgipanl.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fehbvm.com/Article/details/gtioyztyc.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.hesvh.cn/Article/details/gtugkxmsg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.zdbjq.cn/Article/details/gjbumozzq.sHtML

[S10] C：指针与解引用
来源：http://wap.zdbjq.cn/Article/details/gzzofliep.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.hesvh.cn/Article/details/gcrhzwfrx.sHtML

[S11] C：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gqxlxocgn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fehbvm.com/Article/details/ggvpzciqk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.hesvh.cn/Article/details/ggaqnwfsf.sHtML

fclose(f);
来源：http://baike.fehbvm.com/Article/details/gyypmxxsg.sHtML

[S12] C：写文件
来源：http://m.share.fehbvm.com/Article/details/giwwyltok.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fehbvm.com/Article/details/gehnsrjum.sHtML

[S13] C：宏定义
来源：http://blog.fehbvm.com/Article/details/gikyqghsa.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fehbvm.com/Article/details/ggagwiuch.sHtML

[S14] C：枚举
来源：http://www.share.fehbvm.com/Article/details/ghfpjnwbq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.zdbjq.cn/Article/details/gnurfdsua.sHtML

[S15] C：类型转换
来源：http://m.share.hesvh.cn/Article/details/gjdelmsbi.sHtML

(double) a / b
来源：http://baike.zdbjq.cn/Article/details/ghhrtxnur.sHtML

[S16] C：位操作置位
来源：http://www.share.hesvh.cn/Article/details/guwtqucvb.sHtML

x |= (1 << 3);
来源：http://www.m.share.hesvh.cn/Article/details/gupnshvph.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gyjlwusbk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.hesvh.cn/Article/details/gqvvxittf.sHtML

[S18] C：命令行参数
来源：http://m.share.zdbjq.cn/Article/details/gcukorxfr.sHtML

int main(int argc, char **argv)
来源：http://www.share.hesvh.cn/Article/details/gdieipjfu.sHtML

[S19] C：快速排序
来源：http://www.m.share.hesvh.cn/Article/details/gyajxzvxe.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/gwioxspeb.sHtML

[S20] C：二分查找
来源：http://3g.fehbvm.com/Article/details/gtxylbohu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/gjvpclfps.sHtML

[S21] C：字符类别判断
来源：http://www.share.zdbjq.cn/Article/details/gmahnxush.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fehbvm.com/Article/details/gkywjstbb.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/gyekdbvqt.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fehbvm.com/Article/details/gdqrltgtc.sHtML

[S23] C：随机数
来源：http://3g.zdbjq.cn/Article/details/gvmskyoxs.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.hesvh.cn/Article/details/grqjcxmgh.sHtML

[S24] C：获取本地时间
来源：http://3g.zdbjq.cn/Article/details/gpphkrttl.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.zdbjq.cn/Article/details/gyvirrbzl.sHtML

[S25] C：内存拷贝
来源：http://read.share.fehbvm.com/Article/details/gcjiwojpj.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fehbvm.com/Article/details/gheglvfrd.sHtML

[S26] C：内存清零
来源：http://www.m.share.zdbjq.cn/Article/details/gakpfvqgw.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.zdbjq.cn/Article/details/gwcjegjbf.sHtML

[S27] C：定义常量
来源：http://mobile.zdbjq.cn/Article/details/gjukbvoxw.sHtML

const double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gfdnlzlxr.sHtML

[S28] C：静态变量
来源：http://3g.zdbjq.cn/Article/details/gnwbrvvdg.sHtML

static int counter = 0;
来源：http://www.m.share.hesvh.cn/Article/details/gdkafarvf.sHtML

[S29] C：变参函数
来源：http://wap.hesvh.cn/Article/details/gemavaaic.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fehbvm.com/Article/details/gwlfeemah.sHtML

[S30] C：头文件保护
来源：http://3g.fehbvm.com/Article/details/gqqalxbaq.sHtML

#ifndef X_H
来源：http://www.share.hesvh.cn/Article/details/gbftvlzgd.sHtML

#define X_H
来源：http://m.share.fehbvm.com/Article/details/gxbhyvdhm.sHtML

#endif
来源：http://mobile.fehbvm.com/Article/details/gdzqhqfku.sHtML

[S31] C++：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gupqivrur.sHtML

#include <iostream>
来源：http://baike.zdbjq.cn/Article/details/gxzdqiwdl.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.zdbjq.cn/Article/details/gpmrepcbj.sHtML

[S32] C++：字符串
来源：http://mobile.zdbjq.cn/Article/details/gbnwahrvz.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.hesvh.cn/Article/details/gtwzepbhm.sHtML

[S33] C++：vector 增删
来源：http://m.share.hesvh.cn/Article/details/gxsbujgjj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gawmalvwx.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fehbvm.com/Article/details/gppnwnnpk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.zdbjq.cn/Article/details/ghcthkycx.sHtML

[S35] C++：map
来源：http://www.share.zdbjq.cn/Article/details/gnyczggpk.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/ghjxsnpvw.sHtML

[S36] C++：unordered_map
来源：http://read.share.fehbvm.com/Article/details/gpbiprrqr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gebzkhmbq.sHtML

[S37] C++：set
来源：http://blog.fehbvm.com/Article/details/ghmspdcsy.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.zdbjq.cn/Article/details/gcrowvkiu.sHtML

[S38] C++：排序
来源：http://www.blog.fehbvm.com/Article/details/ghrixuvue.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/gnfahtcny.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.zdbjq.cn/Article/details/givxjbgsp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.zdbjq.cn/Article/details/grlrbmodg.sHtML

[S40] C++：查找元素
来源：http://blog.fehbvm.com/Article/details/gpkpznqvj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fehbvm.com/Article/details/gocoqsodp.sHtML

[S41] C++：类与构造函数
来源：http://wap.zdbjq.cn/Article/details/gtnscgkzi.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.hesvh.cn/Article/details/glpttspsc.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.hesvh.cn/Article/details/gfzmiuyzk.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.hesvh.cn/Article/details/gomldaapf.sHtML

[S43] C++：智能指针
来源：http://wap.fehbvm.com/Article/details/guynwgasj.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.zdbjq.cn/Article/details/gcwpijkgo.sHtML

[S44] C++：引用传参
来源：http://www.m.share.hesvh.cn/Article/details/gtzujihcd.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fehbvm.com/Article/details/gfnoupveu.sHtML

[S45] C++：lambda
来源：http://www.m.share.fehbvm.com/Article/details/gvxsehjih.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.hesvh.cn/Article/details/grouzayiy.sHtML

[S46] C++：函数模板
来源：http://wap.hesvh.cn/Article/details/gyyydrakv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.hesvh.cn/Article/details/grphwuezm.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.hesvh.cn/Article/details/gyamdvjtj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fehbvm.com/Article/details/gajztdwzv.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gysmnxyjz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.zdbjq.cn/Article/details/gtaevdwbz.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fehbvm.com/Article/details/gbkdaopjf.sHtML

[S49] C++：写文件
来源：http://wap.fehbvm.com/Article/details/gjtobezvg.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.zdbjq.cn/Article/details/gyqospyqh.sHtML

[S50] C++：格式化数字
来源：http://www.blog.hesvh.cn/Article/details/gqrdtkusb.sHtML


<!-- 参考信息 -->