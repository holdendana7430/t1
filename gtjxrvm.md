代发 wailian999

SHOW INDEX FROM users;
来源：http://3g.hesvh.cn/Article/details/geiossgnq.sHtML

[Q73] 查看表状态
来源：http://baike.zdbjq.cn/Article/details/gsnolilyo.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.hesvh.cn/Article/details/gwxcwebvm.sHtML

[Q74] 强制使用索引
来源：http://read.share.zdbjq.cn/Article/details/gqdtuizme.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.hesvh.cn/Article/details/gbwbtrrmd.sHtML

[Q75] 日期格式化
来源：http://3g.hesvh.cn/Article/details/gsnpkvyix.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gcffxttnd.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.hesvh.cn/Article/details/gzyqunlbc.sHtML

[Q76] 按天统计
来源：http://3g.hesvh.cn/Article/details/gmwgnlwbr.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.hesvh.cn/Article/details/gjhvvzywg.sHtML

[Q77] 时间加减
来源：http://www.m.share.zdbjq.cn/Article/details/gbtzpkmtr.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.hesvh.cn/Article/details/geyzwjbye.sHtML

[Q78] 当前时间
来源：http://m.share.zdbjq.cn/Article/details/gxoyerbrs.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.zdbjq.cn/Article/details/ghtrjuokh.sHtML

[Q79] 字符串拼接
来源：http://www.share.fehbvm.com/Article/details/grdmblopl.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fehbvm.com/Article/details/glbpqbkij.sHtML

[Q80] 字符串截取
来源：http://m.share.fehbvm.com/Article/details/gqzllnwpx.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fehbvm.com/Article/details/grzkitsjn.sHtML

[Q81] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/ghplrawdz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gpycfvybf.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.hesvh.cn/Article/details/gqrwngemo.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gclpcdxwa.sHtML

[Q83] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gkitxvgpo.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gsraapinp.sHtML

[Q84] 去除首尾空格
来源：http://blog.hesvh.cn/Article/details/gxhzzsafl.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gljpqodmc.sHtML

[Q85] 数值取整
来源：http://m.share.hesvh.cn/Article/details/ggnzgntek.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.zdbjq.cn/Article/details/glgatefdl.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.hesvh.cn/Article/details/gxcktonnv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.zdbjq.cn/Article/details/gemoffgav.sHtML

[Q87] JSON 字段做条件
来源：http://baike.zdbjq.cn/Article/details/ghclrnmem.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fehbvm.com/Article/details/gajlanxth.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.zdbjq.cn/Article/details/gmseriepn.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.zdbjq.cn/Article/details/gjdbmgxvc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fehbvm.com/Article/details/gwylydzjh.sHtML

[Q89] 判断表是否存在
来源：http://3g.hesvh.cn/Article/details/gbugsihfe.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.hesvh.cn/Article/details/ggjofevlu.sHtML

[Q90] 生成序号列
来源：http://m.share.zdbjq.cn/Article/details/gyxmjfpcb.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.hesvh.cn/Article/details/guffzweev.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gymsejegp.sHtML

R. Bash 专题
来源：http://blog.hesvh.cn/Article/details/glodjhghw.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gaeglplxc.sHtML

[R01] shebang 与严格模式
来源：http://wap.hesvh.cn/Article/details/gdfviclte.sHtML

#!/usr/bin/env bash
来源：http://3g.hesvh.cn/Article/details/gqthvntva.sHtML

set -euo pipefail
来源：http://mobile.hesvh.cn/Article/details/gxzjslgdx.sHtML

[R02] 变量赋值与使用
来源：http://m.share.zdbjq.cn/Article/details/gnkgaxkug.sHtML

name="Tom"; echo "$name"
来源：http://3g.fehbvm.com/Article/details/gwdivlzmf.sHtML

[R03] 只读变量
来源：http://mobile.fehbvm.com/Article/details/gtktnpxgx.sHtML

readonly PI=3.14
来源：http://m.share.fehbvm.com/Article/details/gegohngwd.sHtML

[R04] 位置参数
来源：http://3g.fehbvm.com/Article/details/gmqvzxruf.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fehbvm.com/Article/details/gqczgoyjn.sHtML

[R05] 参数默认值
来源：http://baike.zdbjq.cn/Article/details/gofigjruu.sHtML

name="${1:-default}"
来源：http://mobile.zdbjq.cn/Article/details/gzgpafqjs.sHtML

[R06] 判断命令是否存在
来源：http://read.share.hesvh.cn/Article/details/gjmgphhfp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/gmtnshwqq.sHtML

[R07] if 判断文件
来源：http://www.share.hesvh.cn/Article/details/gkuyllxob.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.zdbjq.cn/Article/details/gbutoinnw.sHtML

[R08] 数值比较
来源：http://3g.zdbjq.cn/Article/details/gmsewvzjb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fehbvm.com/Article/details/gzulguqcv.sHtML

[R09] 字符串比较
来源：http://www.share.fehbvm.com/Article/details/gciwnammn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.hesvh.cn/Article/details/gujmjkamf.sHtML

[R10] 正则匹配
来源：http://3g.zdbjq.cn/Article/details/gjgqaubbc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gresncmgv.sHtML

[R11] case 多分支
来源：http://read.share.fehbvm.com/Article/details/gakcoarfn.sHtML

case "$1" in
来源：http://3g.fehbvm.com/Article/details/gnzukcsbn.sHtML

start) echo "启动" ;;
来源：http://www.share.zdbjq.cn/Article/details/gltmlzhus.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fehbvm.com/Article/details/gpsxxchtv.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fehbvm.com/Article/details/gtxelktut.sHtML

esac
来源：http://www.m.share.fehbvm.com/Article/details/gbkinysji.sHtML

[R12] for 遍历文件
来源：http://www.share.fehbvm.com/Article/details/gonpgumxq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fehbvm.com/Article/details/golmvtsvp.sHtML

[R13] for 计数循环
来源：http://3g.fehbvm.com/Article/details/gxnykvqfx.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/gkzjcygvw.sHtML

[R14] C 风格 for
来源：http://blog.zdbjq.cn/Article/details/gvmlgsqtr.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/gtddqytrj.sHtML

[R15] while 逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gitxuonjs.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.zdbjq.cn/Article/details/grjghlwtf.sHtML

[R16] until 等待条件
来源：http://www.share.hesvh.cn/Article/details/ggpztkoko.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gsbeaiotb.sHtML

[R17] 数组定义与取值
来源：http://baike.zdbjq.cn/Article/details/gxhzxmvoi.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.zdbjq.cn/Article/details/grmzbjrsc.sHtML

[R18] 遍历数组
来源：http://m.share.zdbjq.cn/Article/details/gbabpdndk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.zdbjq.cn/Article/details/gbnupeoon.sHtML

[R19] 数组长度
来源：http://wap.hesvh.cn/Article/details/gtjoyfqss.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fehbvm.com/Article/details/grjxtnxaj.sHtML

[R20] 关联数组（字典）
来源：http://mobile.zdbjq.cn/Article/details/gnmaunhvx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.zdbjq.cn/Article/details/ghcxgyvqk.sHtML

[R21] 字符串长度
来源：http://m.share.zdbjq.cn/Article/details/gwfdmrxte.sHtML

echo "${#s}"
来源：http://www.m.share.hesvh.cn/Article/details/gstjwqsxu.sHtML

[R22] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/guboqsukl.sHtML

echo "${s:0:5}"
来源：http://baike.zdbjq.cn/Article/details/gimknwnnn.sHtML

[R23] 字符串替换
来源：http://3g.fehbvm.com/Article/details/glasvxebq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fehbvm.com/Article/details/glexibznz.sHtML

[R24] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gztgwnrpw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.zdbjq.cn/Article/details/gxrbmfahe.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.hesvh.cn/Article/details/gmovlaqov.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.hesvh.cn/Article/details/gqicolicv.sHtML

[R26] 命令替换
来源：http://www.m.share.fehbvm.com/Article/details/gzbeqtywh.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.hesvh.cn/Article/details/gujspvawf.sHtML

[R27] 算术展开
来源：http://www.m.share.zdbjq.cn/Article/details/gujctzmqe.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fehbvm.com/Article/details/gyjzagoyp.sHtML

[R28] 浮点运算
来源：http://www.share.fehbvm.com/Article/details/gowtlnnfd.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fehbvm.com/Article/details/gwufyrnwy.sHtML

[R29] 定义函数
来源：http://wap.zdbjq.cn/Article/details/gzqaqftob.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fehbvm.com/Article/details/gqqftjlqb.sHtML

[R30] 函数返回状态码
来源：http://read.share.hesvh.cn/Article/details/ggtwcapdw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fehbvm.com/Article/details/grrgrkfxg.sHtML

[R31] 局部变量
来源：http://3g.zdbjq.cn/Article/details/gpnkonzcr.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.zdbjq.cn/Article/details/gxlcrapyh.sHtML

[R32] 参数个数校验
来源：http://mobile.fehbvm.com/Article/details/gjvctksmo.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/guwskhsuj.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.zdbjq.cn/Article/details/gkvbdnbso.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.hesvh.cn/Article/details/gtvajfrhs.sHtML

[R34] 退出时清理
来源：http://wap.zdbjq.cn/Article/details/gvbxuucoy.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gaqjjjvpb.sHtML

[R35] 后台执行并等待
来源：http://m.share.hesvh.cn/Article/details/gvksipnff.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fehbvm.com/Article/details/gjdrhvpif.sHtML

[R36] 并发执行多个任务
来源：http://wap.fehbvm.com/Article/details/gbsiplczd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.hesvh.cn/Article/details/gxfunqelb.sHtML

[R37] 把输出赋给变量
来源：http://3g.fehbvm.com/Article/details/gvtgcsrqc.sHtML

files=$(ls -1)
来源：http://mobile.fehbvm.com/Article/details/galwdtfaf.sHtML

[R38] 管道串联
来源：http://www.blog.fehbvm.com/Article/details/gprhhwmhg.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fehbvm.com/Article/details/ghuyrleiu.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fehbvm.com/Article/details/gsptyhgsb.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/gerpeigis.sHtML

[R40] 追加写日志
来源：http://wap.zdbjq.cn/Article/details/grtkjbkfx.sHtML

echo "log" >> out.log
来源：http://3g.hesvh.cn/Article/details/gencsqtru.sHtML

[R41] 丢弃输出
来源：http://wap.fehbvm.com/Article/details/giemycmbh.sHtML

cmd >/dev/null 2>&1
来源：http://3g.zdbjq.cn/Article/details/gmexhdqfl.sHtML

[R42] 输入重定向
来源：http://read.share.fehbvm.com/Article/details/gcoumvucg.sHtML

wc -l < a.txt
来源：http://wap.zdbjq.cn/Article/details/gqlgegmsu.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.zdbjq.cn/Article/details/gvhlmpywi.sHtML

find . -name "*.log" -type f
来源：http://3g.fehbvm.com/Article/details/gqlsdylac.sHtML

[R44] 按修改时间查找
来源：http://read.share.hesvh.cn/Article/details/gxmfrgast.sHtML

find . -mtime -7 -type f
来源：http://blog.fehbvm.com/Article/details/ghfwogzep.sHtML

[R45] 批量删除
来源：http://baike.zdbjq.cn/Article/details/gvhrrguzn.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.zdbjq.cn/Article/details/gxkpsmyid.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.zdbjq.cn/Article/details/gzmysmqbk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.hesvh.cn/Article/details/gfyfiftwj.sHtML

[R47] sed 单行替换
来源：http://www.m.share.hesvh.cn/Article/details/gjfhbubvf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.hesvh.cn/Article/details/ghxuynhit.sHtML

[R48] awk 取指定列
来源：http://wap.fehbvm.com/Article/details/gjpjnqiji.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gevtflahy.sHtML

[R49] awk 带条件
来源：http://m.share.hesvh.cn/Article/details/ghveammec.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.hesvh.cn/Article/details/gcjykblbd.sHtML

[R50] awk 求和
来源：http://www.blog.hesvh.cn/Article/details/grpdkxaoi.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gmovdhnnn.sHtML

[R51] 排序去重取前几
来源：http://3g.hesvh.cn/Article/details/gpyzuyoqn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fehbvm.com/Article/details/goobydbvq.sHtML

[R52] 统计行数
来源：http://read.share.zdbjq.cn/Article/details/gnuqgomqy.sHtML

wc -l a.txt
来源：http://blog.zdbjq.cn/Article/details/gqacpfbej.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.zdbjq.cn/Article/details/guaulvgnd.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.zdbjq.cn/Article/details/gyuwmlrce.sHtML

[R54] 比较两个文件
来源：http://m.share.fehbvm.com/Article/details/gkaumnlhj.sHtML

diff a.txt b.txt
来源：http://blog.hesvh.cn/Article/details/gwrmnltyk.sHtML

[R55] 压缩与解压
来源：http://baike.zdbjq.cn/Article/details/grihozyog.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.hesvh.cn/Article/details/ghoumvaof.sHtML

[R56] 远程拷贝
来源：http://read.share.fehbvm.com/Article/details/geyrhbjgp.sHtML

scp file user@host:/path/
来源：http://3g.hesvh.cn/Article/details/gxigpabyc.sHtML

[R57] 远程执行命令
来源：http://read.share.hesvh.cn/Article/details/gkkidutdr.sHtML

ssh user@host 'uptime'
来源：http://3g.hesvh.cn/Article/details/gmvcrhmtk.sHtML

[R58] 下载文件
来源：http://read.share.zdbjq.cn/Article/details/gfuaxadwq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.hesvh.cn/Article/details/gissgunbc.sHtML

[R59] 发 POST JSON
来源：http://blog.zdbjq.cn/Article/details/gswmkejym.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fehbvm.com/Article/details/ghhjjkdrx.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/gpdsktepa.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fehbvm.com/Article/details/gkffwustu.sHtML

[R61] 磁盘占用
来源：http://mobile.zdbjq.cn/Article/details/gqhimuiiw.sHtML

df -h;  du -sh *
来源：http://m.share.hesvh.cn/Article/details/gzcotroze.sHtML

[R62] 找最占空间的文件
来源：http://mobile.zdbjq.cn/Article/details/gelznhwru.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.zdbjq.cn/Article/details/glhlhpdwv.sHtML

[R63] 内存与进程
来源：http://blog.fehbvm.com/Article/details/gnxppnrtl.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fehbvm.com/Article/details/gqvsmvfwq.sHtML

[R64] 结束进程
来源：http://m.share.hesvh.cn/Article/details/gavnwauvo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.hesvh.cn/Article/details/gobyplnbv.sHtML

[R65] 查看端口占用
来源：http://mobile.fehbvm.com/Article/details/gmwyemdqi.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.hesvh.cn/Article/details/grbxvpsex.sHtML

[R66] 定时任务
来源：http://m.share.zdbjq.cn/Article/details/gxvmfqsul.sHtML

crontab -e;  crontab -l
来源：http://mobile.hesvh.cn/Article/details/ggxlfmsdp.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.hesvh.cn/Article/details/gtnbnfmws.sHtML

openssl rand -hex 16
来源：http://www.share.fehbvm.com/Article/details/gfbohsqxj.sHtML

[R68] 计算文件校验值
来源：http://www.share.fehbvm.com/Article/details/gdprldnel.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gayzqbrgg.sHtML

[R69] 生成随机密码
来源：http://www.blog.fehbvm.com/Article/details/gumxuplqn.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.hesvh.cn/Article/details/gcdvghwol.sHtML

[R70] 时间戳与互转
来源：http://www.blog.hesvh.cn/Article/details/gqpmvxjaf.sHtML

date +%s;  date -d @1700000000
来源：http://blog.zdbjq.cn/Article/details/gixwswiwj.sHtML

[R71] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/ghbrrgvvx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.zdbjq.cn/Article/details/gjyjojpla.sHtML

[R72] 等待端口就绪
来源：http://mobile.fehbvm.com/Article/details/gcvxpjyoa.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/gxdnljour.sHtML

[R73] 分割大日志
来源：http://www.m.share.hesvh.cn/Article/details/gmmgxxhhy.sHtML

split -l 1000 big.log part_
来源：http://www.blog.hesvh.cn/Article/details/gnnotesww.sHtML

[R74] 批量重命名
来源：http://blog.hesvh.cn/Article/details/glqmtauyv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.hesvh.cn/Article/details/gmbhnvlgn.sHtML

[R75] 导出环境变量
来源：http://m.share.fehbvm.com/Article/details/gwencorsg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fehbvm.com/Article/details/gcinbtoko.sHtML

[R76] 使用临时文件
来源：http://3g.fehbvm.com/Article/details/gegqhybhr.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/ghgbxivim.sHtML

[R77] 读取用户输入
来源：http://baike.zdbjq.cn/Article/details/gpkhbfppf.sHtML

read -rp "请输入: " ans
来源：http://baike.fehbvm.com/Article/details/gwoaymckm.sHtML

[R78] 交互式菜单
来源：http://m.share.zdbjq.cn/Article/details/gujbrgmqa.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.hesvh.cn/Article/details/gebilhynv.sHtML

[R79] 解析命令行选项
来源：http://www.blog.hesvh.cn/Article/details/gatponwxd.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.hesvh.cn/Article/details/glhndyrke.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.hesvh.cn/Article/details/gxjfdxnqy.sHtML

time ./run.sh
来源：http://blog.fehbvm.com/Article/details/gtxkdpssb.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gmulanqkg.sHtML

S. C / C++ 专题
来源：http://www.share.fehbvm.com/Article/details/gmpwlttpa.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gonzdsdqg.sHtML

[S01] C：Hello World
来源：http://read.share.hesvh.cn/Article/details/gkuxhemmj.sHtML

#include <stdio.h>
来源：http://www.share.hesvh.cn/Article/details/gsdkkkezf.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.zdbjq.cn/Article/details/ghgvgatnk.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fehbvm.com/Article/details/gcvefoklq.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fehbvm.com/Article/details/gujozigbv.sHtML

[S03] C：读入整数
来源：http://www.blog.hesvh.cn/Article/details/gzdwrhoqw.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fehbvm.com/Article/details/ggatydqin.sHtML

[S04] C：字符串复制
来源：http://3g.zdbjq.cn/Article/details/gvvugaihv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gydoeesom.sHtML

[S05] C：字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/gyjtdbopp.sHtML

strlen(s)
来源：http://m.share.zdbjq.cn/Article/details/gstdlrcmp.sHtML

[S06] C：字符串比较
来源：http://mobile.hesvh.cn/Article/details/ghwfbfwkl.sHtML

strcmp(a, b) == 0
来源：http://mobile.zdbjq.cn/Article/details/gpqktwegi.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fehbvm.com/Article/details/gjukfkzjc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fehbvm.com/Article/details/ghsgpunpn.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.hesvh.cn/Article/details/gmbzbvrdo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fehbvm.com/Article/details/gcdgymozr.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.hesvh.cn/Article/details/gwpdylkae.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fehbvm.com/Article/details/gfekwxyfr.sHtML

[S10] C：指针与解引用
来源：http://wap.fehbvm.com/Article/details/gkszfvtmy.sHtML

int *p = &a;  *p = 5;
来源：http://wap.zdbjq.cn/Article/details/gewtaalhp.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/glakxnpgn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.hesvh.cn/Article/details/gytqpndwi.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fehbvm.com/Article/details/gcerldxve.sHtML

fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gigcxqsfa.sHtML

[S12] C：写文件
来源：http://blog.hesvh.cn/Article/details/gphiryyrk.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.zdbjq.cn/Article/details/gauptcmap.sHtML

[S13] C：宏定义
来源：http://www.blog.hesvh.cn/Article/details/gtmhgqkim.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.hesvh.cn/Article/details/giwemnsmd.sHtML

[S14] C：枚举
来源：http://mobile.zdbjq.cn/Article/details/gaoehzwtw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.hesvh.cn/Article/details/gelyxwfih.sHtML

[S15] C：类型转换
来源：http://baike.fehbvm.com/Article/details/gyiehdfhj.sHtML

(double) a / b
来源：http://www.share.fehbvm.com/Article/details/grrdvozpk.sHtML

[S16] C：位操作置位
来源：http://www.share.hesvh.cn/Article/details/gycukdzbb.sHtML

x |= (1 << 3);
来源：http://3g.hesvh.cn/Article/details/gycioctgp.sHtML

[S17] C：安全拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gmhnrqhav.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.zdbjq.cn/Article/details/gfnngsiuj.sHtML

[S18] C：命令行参数
来源：http://wap.zdbjq.cn/Article/details/giaorzqew.sHtML

int main(int argc, char **argv)
来源：http://read.share.hesvh.cn/Article/details/gxianhvvt.sHtML

[S19] C：快速排序
来源：http://m.share.fehbvm.com/Article/details/gzdbkibzl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/ghtvdziwz.sHtML

[S20] C：二分查找
来源：http://baike.hesvh.cn/Article/details/gvbvhcykr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/gwowojcfe.sHtML

[S21] C：字符类别判断
来源：http://3g.zdbjq.cn/Article/details/gdlmxjjqa.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.hesvh.cn/Article/details/gagluakwn.sHtML

[S22] C：字符串转数字
来源：http://m.share.fehbvm.com/Article/details/grdhyvtmi.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.hesvh.cn/Article/details/guwkmirpo.sHtML

[S23] C：随机数
来源：http://www.blog.fehbvm.com/Article/details/gymwmfyps.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.zdbjq.cn/Article/details/gaoraawtn.sHtML

[S24] C：获取本地时间
来源：http://read.share.zdbjq.cn/Article/details/gfbzfpukn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.zdbjq.cn/Article/details/gejbgntdu.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gcavltjrv.sHtML

memcpy(dst, src, n);
来源：http://blog.hesvh.cn/Article/details/gnemheisx.sHtML

[S26] C：内存清零
来源：http://3g.fehbvm.com/Article/details/guzyaehan.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fehbvm.com/Article/details/gddxkafrp.sHtML

[S27] C：定义常量
来源：http://www.blog.hesvh.cn/Article/details/gwztrbppo.sHtML

const double PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/guhiqmthz.sHtML

[S28] C：静态变量
来源：http://www.share.fehbvm.com/Article/details/gwkfdvdei.sHtML

static int counter = 0;
来源：http://wap.zdbjq.cn/Article/details/gtspclceq.sHtML

[S29] C：变参函数
来源：http://read.share.fehbvm.com/Article/details/gkuaicrmf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.hesvh.cn/Article/details/gkzvitmjr.sHtML

[S30] C：头文件保护
来源：http://read.share.fehbvm.com/Article/details/gkchaifte.sHtML

#ifndef X_H
来源：http://3g.zdbjq.cn/Article/details/gbqvltsii.sHtML

#define X_H
来源：http://www.m.share.hesvh.cn/Article/details/gbwtzyclr.sHtML

#endif
来源：http://m.share.fehbvm.com/Article/details/gsbozmqqo.sHtML

[S31] C++：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gtwaiklie.sHtML

#include <iostream>
来源：http://m.share.fehbvm.com/Article/details/gmzgsrdwz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fehbvm.com/Article/details/gffahrstk.sHtML

[S32] C++：字符串
来源：http://www.blog.hesvh.cn/Article/details/gchaoxsih.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.hesvh.cn/Article/details/gruhbrlrt.sHtML

[S33] C++：vector 增删
来源：http://read.share.zdbjq.cn/Article/details/gxcemnxeq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.zdbjq.cn/Article/details/gtzupcadz.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fehbvm.com/Article/details/gvhsjrnpn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fehbvm.com/Article/details/gbzbzfqrn.sHtML

[S35] C++：map
来源：http://www.blog.fehbvm.com/Article/details/gkcfyqifr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/grxwhrgym.sHtML

[S36] C++：unordered_map
来源：http://www.share.hesvh.cn/Article/details/grgkbgssu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gspxkxpos.sHtML

[S37] C++：set
来源：http://www.blog.fehbvm.com/Article/details/geplipwyh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fehbvm.com/Article/details/gikiyilbt.sHtML

[S38] C++：排序
来源：http://3g.zdbjq.cn/Article/details/gcjtlilhr.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.zdbjq.cn/Article/details/gupcfdbeq.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.hesvh.cn/Article/details/gzzhtnlln.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fehbvm.com/Article/details/grrfnuemf.sHtML

[S40] C++：查找元素
来源：http://3g.zdbjq.cn/Article/details/gcvbagqbd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fehbvm.com/Article/details/gdbeifrbo.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fehbvm.com/Article/details/gdrikjcgu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.zdbjq.cn/Article/details/gqatjkucn.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.zdbjq.cn/Article/details/govkohudy.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.hesvh.cn/Article/details/gqknfxwhw.sHtML


<!-- 参考信息 -->