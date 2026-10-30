代发 wailian999

[Q84] 去除首尾空格
来源：http://blog.fanxiaobao.xyz/Article/details/gzikttpjf.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gtguxhokh.sHtML

[Q85] 数值取整
来源：http://mobile.fanxiaobao.xyz/Article/details/gcngsphyr.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fanxiaobao.xyz/Article/details/gixufvlqv.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gassskkmk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fanxiaobao.xyz/Article/details/gclgkwsce.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gfrnjdyum.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gadrmdqmh.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fanxiaobao.xyz/Article/details/grcgedhth.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fanxiaobao.xyz/Article/details/gczlyjuqo.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnvgixlfw.sHtML

[Q89] 判断表是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gunoaklot.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gsebghqqk.sHtML

[Q90] 生成序号列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxjojger.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fanxiaobao.xyz/Article/details/gmfviizrr.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gmsidjwzh.sHtML

R. Bash 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gjedatiny.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gdthpniag.sHtML

[R01] shebang 与严格模式
来源：http://wap.fanxiaobao.xyz/Article/details/gzkqrcgww.sHtML

#!/usr/bin/env bash
来源：http://www.share.fanxiaobao.xyz/Article/details/gcjibuynr.sHtML

set -euo pipefail
来源：http://baike.fanxiaobao.xyz/Article/details/gzuohpqiy.sHtML

[R02] 变量赋值与使用
来源：http://3g.fanxiaobao.xyz/Article/details/gabvkchlg.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gdthloqgh.sHtML

[R03] 只读变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gcstzotji.sHtML

readonly PI=3.14
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjpptupf.sHtML

[R04] 位置参数
来源：http://wap.fanxiaobao.xyz/Article/details/gbmsjndyj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fanxiaobao.xyz/Article/details/gdbcwklze.sHtML

[R05] 参数默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gasqdmudk.sHtML

name="${1:-default}"
来源：http://wap.fanxiaobao.xyz/Article/details/gpveprlaa.sHtML

[R06] 判断命令是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gxmbarsxp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdywollvo.sHtML

[R07] if 判断文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmiykfyi.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/grsvxaviq.sHtML

[R08] 数值比较
来源：http://3g.fanxiaobao.xyz/Article/details/giaiptagy.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/geevlqljq.sHtML

[R09] 字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/grglamafo.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gepqttetp.sHtML

[R10] 正则匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvjtvrexo.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gikjufztp.sHtML

[R11] case 多分支
来源：http://www.blog.fanxiaobao.xyz/Article/details/grswjdjlb.sHtML

case "$1" in
来源：http://wap.fanxiaobao.xyz/Article/details/gvalgkyfe.sHtML

start) echo "启动" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gesscidyk.sHtML

stop)  echo "停止" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gcdqrtoum.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gimucfmau.sHtML

esac
来源：http://mobile.fanxiaobao.xyz/Article/details/grlvjeesi.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giishlxmg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gwdpqpepo.sHtML

[R13] for 计数循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvotpfwrx.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gwugbbjzs.sHtML

[R14] C 风格 for
来源：http://blog.fanxiaobao.xyz/Article/details/grktonqzc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gtpsqpyns.sHtML

[R15] while 逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gwsgvkxuq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gpbmnflbo.sHtML

[R16] until 等待条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdpjmzqs.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gfqqwiftf.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fanxiaobao.xyz/Article/details/guibembza.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gpuhvchzi.sHtML

[R18] 遍历数组
来源：http://wap.fanxiaobao.xyz/Article/details/gofhxryhn.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/geczfofxh.sHtML

[R19] 数组长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gioayxynq.sHtML

echo "${#arr[@]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gfjknhqbr.sHtML

[R20] 关联数组（字典）
来源：http://baike.fanxiaobao.xyz/Article/details/gwviqtmgr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gyvyrxqnc.sHtML

[R21] 字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gqgatsmit.sHtML

echo "${#s}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gtsxomzdp.sHtML

[R22] 截取子串
来源：http://m.share.fanxiaobao.xyz/Article/details/geuckogpd.sHtML

echo "${s:0:5}"
来源：http://m.share.fanxiaobao.xyz/Article/details/geefhcgtx.sHtML

[R23] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gixqxlnbt.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gmkotkgca.sHtML

[R24] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxcfvops.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fanxiaobao.xyz/Article/details/givxszmdq.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fanxiaobao.xyz/Article/details/gqqwyyudh.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fanxiaobao.xyz/Article/details/gccaviahc.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gjyelxtuh.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fanxiaobao.xyz/Article/details/gnlpkmvwx.sHtML

[R27] 算术展开
来源：http://wap.fanxiaobao.xyz/Article/details/gsifmdded.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gquzykpge.sHtML

[R28] 浮点运算
来源：http://mobile.fanxiaobao.xyz/Article/details/gkwklelde.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpoegzdrr.sHtML

[R29] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gjqlfzpui.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/gawmfwawz.sHtML

[R30] 函数返回状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gffvcgify.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkqhuzdgu.sHtML

[R31] 局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/ggyaglwfz.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjodxvouh.sHtML

[R32] 参数个数校验
来源：http://wap.fanxiaobao.xyz/Article/details/gkiivdqta.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gkhycsrfe.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fanxiaobao.xyz/Article/details/gqsodktkl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fanxiaobao.xyz/Article/details/gywekyjri.sHtML

[R34] 退出时清理
来源：http://3g.fanxiaobao.xyz/Article/details/ggydjvurl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmzmiaxp.sHtML

[R35] 后台执行并等待
来源：http://3g.fanxiaobao.xyz/Article/details/gbdqicrix.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfzzsmofn.sHtML

[R36] 并发执行多个任务
来源：http://3g.fanxiaobao.xyz/Article/details/gcbexrbzs.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fanxiaobao.xyz/Article/details/gphgkakzs.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fanxiaobao.xyz/Article/details/grnjfpshl.sHtML

files=$(ls -1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gztjyqvaq.sHtML

[R38] 管道串联
来源：http://baike.fanxiaobao.xyz/Article/details/gnxnsnaoc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fanxiaobao.xyz/Article/details/ghjewaski.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fanxiaobao.xyz/Article/details/gidkapqrj.sHtML

cmd > out.log 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/ghgnjanos.sHtML

[R40] 追加写日志
来源：http://wap.fanxiaobao.xyz/Article/details/gslsvuibc.sHtML

echo "log" >> out.log
来源：http://3g.fanxiaobao.xyz/Article/details/ggioftdgb.sHtML

[R41] 丢弃输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gpiracxfz.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gwhvvhued.sHtML

[R42] 输入重定向
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpllxnunz.sHtML

wc -l < a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gmbqymaoi.sHtML

[R43] 按名字查找文件
来源：http://www.share.fanxiaobao.xyz/Article/details/ghkykjqbs.sHtML

find . -name "*.log" -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gbnnfxdll.sHtML

[R44] 按修改时间查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gulxgfqwo.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gtqrhtcuu.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzmjrwvvk.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnglwqxk.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fanxiaobao.xyz/Article/details/gfshlczpz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fanxiaobao.xyz/Article/details/gaanugkju.sHtML

[R47] sed 单行替换
来源：http://wap.fanxiaobao.xyz/Article/details/ghlywnldb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gxytuidib.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gciwjybkv.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gsreblebu.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gqeizikut.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fanxiaobao.xyz/Article/details/gxjtqmwwa.sHtML

[R50] awk 求和
来源：http://baike.fanxiaobao.xyz/Article/details/gackmipxs.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gtbuacoaq.sHtML

[R51] 排序去重取前几
来源：http://mobile.fanxiaobao.xyz/Article/details/gmveksyov.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fanxiaobao.xyz/Article/details/grmqfabwd.sHtML

[R52] 统计行数
来源：http://mobile.fanxiaobao.xyz/Article/details/gswkbvwok.sHtML

wc -l a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gipjqltjt.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fanxiaobao.xyz/Article/details/gwyzvkdbw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fanxiaobao.xyz/Article/details/gfdekwxie.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkxoxvfah.sHtML

diff a.txt b.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gytlnstvj.sHtML

[R55] 压缩与解压
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwhmoybde.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fanxiaobao.xyz/Article/details/girnakobf.sHtML

[R56] 远程拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gjqtnvryb.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/gbggfihtz.sHtML

[R57] 远程执行命令
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnlsbsknq.sHtML

ssh user@host 'uptime'
来源：http://mobile.fanxiaobao.xyz/Article/details/gvqgiyqgg.sHtML

[R58] 下载文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gktjzkeah.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fanxiaobao.xyz/Article/details/gkfwpsbgd.sHtML

[R59] 发 POST JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gfscxynfn.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gnnqsxkjk.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gvuhlkkqx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fanxiaobao.xyz/Article/details/grzeanqyr.sHtML

[R61] 磁盘占用
来源：http://wap.fanxiaobao.xyz/Article/details/gyalmfrxk.sHtML

df -h;  du -sh *
来源：http://blog.fanxiaobao.xyz/Article/details/gezqusxzv.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gsyhqpkvu.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fanxiaobao.xyz/Article/details/gnmfzkzqi.sHtML

[R63] 内存与进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gywvltejg.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fanxiaobao.xyz/Article/details/gcortpztv.sHtML

[R64] 结束进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gtbstfmma.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrlzychn.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnxsfgnki.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fanxiaobao.xyz/Article/details/grqbovvlz.sHtML

[R66] 定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gvtjdxvqa.sHtML

crontab -e;  crontab -l
来源：http://blog.fanxiaobao.xyz/Article/details/gwuxdzfto.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fanxiaobao.xyz/Article/details/griypkiyl.sHtML

openssl rand -hex 16
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdomhojjc.sHtML

[R68] 计算文件校验值
来源：http://baike.fanxiaobao.xyz/Article/details/ghxkpvneg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxxchvxc.sHtML

[R69] 生成随机密码
来源：http://www.share.fanxiaobao.xyz/Article/details/goropkljx.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fanxiaobao.xyz/Article/details/glyqwoobq.sHtML

[R70] 时间戳与互转
来源：http://read.share.fanxiaobao.xyz/Article/details/ghpcnoliq.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmqdlshaq.sHtML

[R71] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gdobwyudv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gznjbqiiy.sHtML

[R72] 等待端口就绪
来源：http://baike.fanxiaobao.xyz/Article/details/gdrtdepre.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gpahdzyvt.sHtML

[R73] 分割大日志
来源：http://blog.fanxiaobao.xyz/Article/details/gewrynwkc.sHtML

split -l 1000 big.log part_
来源：http://read.share.fanxiaobao.xyz/Article/details/gopqacpfa.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/gsrzwbymk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gedhdlzet.sHtML

[R75] 导出环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/glhmszcpj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fanxiaobao.xyz/Article/details/gpvfjgkah.sHtML

[R76] 使用临时文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gymaqzwkh.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/ghrlbvusi.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyeebqkqz.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqmktxdnb.sHtML

[R78] 交互式菜单
来源：http://www.share.fanxiaobao.xyz/Article/details/grfxefroz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gtjxvezjj.sHtML

[R79] 解析命令行选项
来源：http://www.share.fanxiaobao.xyz/Article/details/gitnfwaha.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gywcawzud.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/geumddyzt.sHtML

time ./run.sh
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzieyppv.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gcffoblwv.sHtML

S. C / C++ 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/ggieujadc.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gigufppaq.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxcugpsob.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/geckwsjqb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwzajnoar.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/guaetokfm.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fanxiaobao.xyz/Article/details/guuuoamhw.sHtML

[S03] C：读入整数
来源：http://3g.fanxiaobao.xyz/Article/details/gseuzvuiv.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fanxiaobao.xyz/Article/details/gynupmmfx.sHtML

[S04] C：字符串复制
来源：http://mobile.fanxiaobao.xyz/Article/details/gqziwqdaf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbliatbks.sHtML

[S05] C：字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gdmrwesir.sHtML

strlen(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpfqbgfsl.sHtML

[S06] C：字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gmxkqrabm.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjlxinhb.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guoquvbti.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/glrfmhrjw.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fanxiaobao.xyz/Article/details/ghwvvtfjo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fanxiaobao.xyz/Article/details/girjvmmoy.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fanxiaobao.xyz/Article/details/gjmhounlv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fanxiaobao.xyz/Article/details/gwrmqenxc.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwratusvg.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/grmyayutf.sHtML

[S11] C：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gvzelanwj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/gufrohcit.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grmolizru.sHtML

fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpuveeyxx.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gyrmoudjo.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gvwrbmxqi.sHtML

[S13] C：宏定义
来源：http://baike.fanxiaobao.xyz/Article/details/glapmrwuh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavwokenl.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/graqkhlfg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fanxiaobao.xyz/Article/details/guhjpuurv.sHtML

[S15] C：类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gmrylxzek.sHtML

(double) a / b
来源：http://m.share.fanxiaobao.xyz/Article/details/ggejgmzir.sHtML

[S16] C：位操作置位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixzbbggx.sHtML

x |= (1 << 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/goilldnae.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gbhrajqct.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fanxiaobao.xyz/Article/details/gxrdltcal.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grygpychc.sHtML

int main(int argc, char **argv)
来源：http://mobile.fanxiaobao.xyz/Article/details/gckavlxtg.sHtML

[S19] C：快速排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyikvkqbe.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/glsueahnd.sHtML

[S20] C：二分查找
来源：http://baike.fanxiaobao.xyz/Article/details/gwwrmdhjv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/ggcisqumv.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtwiiwesf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fanxiaobao.xyz/Article/details/gukocpucw.sHtML

[S22] C：字符串转数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gqcwyiucu.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpesuwdhn.sHtML

[S23] C：随机数
来源：http://blog.fanxiaobao.xyz/Article/details/ggrrzpqka.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvutpbbg.sHtML

[S24] C：获取本地时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gfiooicad.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvayqyari.sHtML

[S25] C：内存拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gnjkkmout.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsewqwzts.sHtML

[S26] C：内存清零
来源：http://blog.fanxiaobao.xyz/Article/details/gvwkobhwb.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjbxyylk.sHtML

[S27] C：定义常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gnaaarjav.sHtML

const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gdhtpfrni.sHtML

[S28] C：静态变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gqjqcgpjw.sHtML

static int counter = 0;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbegtibzv.sHtML

[S29] C：变参函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gvpcribsc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geuvzmghd.sHtML

[S30] C：头文件保护
来源：http://www.share.fanxiaobao.xyz/Article/details/gzfqxgnbk.sHtML

#ifndef X_H
来源：http://wap.fanxiaobao.xyz/Article/details/ghgiojtmq.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gmndskdob.sHtML

#endif
来源：http://baike.fanxiaobao.xyz/Article/details/gexrohxch.sHtML

[S31] C++：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gynedsyqd.sHtML

#include <iostream>
来源：http://read.share.fanxiaobao.xyz/Article/details/grsndztip.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gricbbyxm.sHtML

[S32] C++：字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gjftfprcm.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fanxiaobao.xyz/Article/details/gerfhcdpa.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtdugygps.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gvtzlkdyo.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fanxiaobao.xyz/Article/details/guvwtjtjo.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gofwbxxqj.sHtML

[S35] C++：map
来源：http://wap.fanxiaobao.xyz/Article/details/gdcpnohvk.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/grbgnjetb.sHtML

[S36] C++：unordered_map
来源：http://blog.fanxiaobao.xyz/Article/details/gzaelqxhr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdcdduwsj.sHtML

[S37] C++：set
来源：http://blog.fanxiaobao.xyz/Article/details/gchbungnp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gccuikuvw.sHtML

[S38] C++：排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gtgjjqiwp.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gffyxpbtf.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbkbropwu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxlekplh.sHtML

[S40] C++：查找元素
来源：http://3g.fanxiaobao.xyz/Article/details/gelmxwhnf.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdzxqfeof.sHtML

[S41] C++：类与构造函数
来源：http://baike.fanxiaobao.xyz/Article/details/ggyqrdcrk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmvwiqszc.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gukwfkzqd.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fanxiaobao.xyz/Article/details/gyzhixvxa.sHtML

[S43] C++：智能指针
来源：http://mobile.fanxiaobao.xyz/Article/details/gwexhujhk.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxnjvfod.sHtML

[S44] C++：引用传参
来源：http://m.share.fanxiaobao.xyz/Article/details/gvdwiqvyp.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gizdkteok.sHtML

[S45] C++：lambda
来源：http://www.blog.fanxiaobao.xyz/Article/details/gholougsw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbfyhnws.sHtML

[S46] C++：函数模板
来源：http://3g.fanxiaobao.xyz/Article/details/gocxsrggm.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gagbpjvdq.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/glujfnfsw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glkpzviof.sHtML

[S48] C++：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gkltwsvoa.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gztvaygrd.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gvtaltirg.sHtML

[S49] C++：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gvlwmymvm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/gzugdzufp.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdnymbmoy.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gpuvpbqyy.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhpaudrz.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gecelvukg.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fanxiaobao.xyz/Article/details/gkwbsnvxz.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fanxiaobao.xyz/Article/details/gpinkroxt.sHtML

[S53] C++：移动语义
来源：http://read.share.fanxiaobao.xyz/Article/details/gcncvrtur.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gafolsshx.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtvburmxx.sHtML


<!-- 参考信息 -->