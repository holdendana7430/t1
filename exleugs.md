代发 wailian999

[Q65] 回滚事务
来源：http://baike.hesvh.cn/Article/details/gwnwtzoiw.sHtML

ROLLBACK;
来源：http://mobile.hesvh.cn/Article/details/gaqjwmjqk.sHtML

[Q66] 行锁查询
来源：http://baike.fehbvm.com/Article/details/gkobrnbbn.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.zdbjq.cn/Article/details/gumyldbrj.sHtML

[Q67] 设置隔离级别
来源：http://m.share.hesvh.cn/Article/details/ghiqzkmth.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fehbvm.com/Article/details/gmolpxxub.sHtML

[Q68] 保存点
来源：http://3g.zdbjq.cn/Article/details/gbtwdhixb.sHtML

SAVEPOINT sp1;
来源：http://m.share.hesvh.cn/Article/details/gtdevsnbo.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fehbvm.com/Article/details/gbvofxdxq.sHtML

[Q69] 查看执行计划
来源：http://3g.zdbjq.cn/Article/details/grfykngbb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.hesvh.cn/Article/details/gaakzaxre.sHtML

[Q70] 更新统计信息
来源：http://blog.hesvh.cn/Article/details/gycitcbdp.sHtML

ANALYZE TABLE users;
来源：http://blog.hesvh.cn/Article/details/gmqdbzsuo.sHtML

[Q71] 查看建表语句
来源：http://www.blog.hesvh.cn/Article/details/gdkkchvss.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fehbvm.com/Article/details/gspypnjbt.sHtML

[Q72] 查看索引
来源：http://www.share.fehbvm.com/Article/details/gljigrjcx.sHtML

SHOW INDEX FROM users;
来源：http://read.share.zdbjq.cn/Article/details/givoohdjw.sHtML

[Q73] 查看表状态
来源：http://read.share.fehbvm.com/Article/details/gbeumcwap.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fehbvm.com/Article/details/gtgkrtcqr.sHtML

[Q74] 强制使用索引
来源：http://m.share.fehbvm.com/Article/details/gdprptnoz.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.hesvh.cn/Article/details/garfllfte.sHtML

[Q75] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/gfcrymxbb.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.hesvh.cn/Article/details/gtrihffsg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.zdbjq.cn/Article/details/gnjwgteqs.sHtML

[Q76] 按天统计
来源：http://www.m.share.zdbjq.cn/Article/details/govwldurr.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fehbvm.com/Article/details/gqxyzhghd.sHtML

[Q77] 时间加减
来源：http://www.blog.hesvh.cn/Article/details/ggtxxjtvl.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.hesvh.cn/Article/details/gwraixfae.sHtML

[Q78] 当前时间
来源：http://3g.hesvh.cn/Article/details/gefcmjavf.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fehbvm.com/Article/details/gaysunpnl.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/gxptcettc.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.hesvh.cn/Article/details/galkjvcde.sHtML

[Q80] 字符串截取
来源：http://read.share.zdbjq.cn/Article/details/gtqiejppe.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gvokgcbqr.sHtML

[Q81] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/gsgeobhbs.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.hesvh.cn/Article/details/gxutictva.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.zdbjq.cn/Article/details/geufnbofn.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gvysqmkvo.sHtML

[Q83] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/ghqkcpdzj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gjxioejdu.sHtML

[Q84] 去除首尾空格
来源：http://3g.zdbjq.cn/Article/details/gnrtjsbsg.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gmcetjswu.sHtML

[Q85] 数值取整
来源：http://baike.hesvh.cn/Article/details/gvohhfbko.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.hesvh.cn/Article/details/gbxmniwcw.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.hesvh.cn/Article/details/gfpadonok.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fehbvm.com/Article/details/goapqieyg.sHtML

[Q87] JSON 字段做条件
来源：http://baike.zdbjq.cn/Article/details/gqujecdvb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.zdbjq.cn/Article/details/gcnrsyiuo.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fehbvm.com/Article/details/glxzbemcn.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fehbvm.com/Article/details/gmeeeqlau.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.zdbjq.cn/Article/details/gsvxqvusk.sHtML

[Q89] 判断表是否存在
来源：http://read.share.hesvh.cn/Article/details/ggsfntzfe.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.zdbjq.cn/Article/details/ghevhkfbj.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fehbvm.com/Article/details/gbsixsxgx.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.zdbjq.cn/Article/details/gdztppwpb.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ggavorbqv.sHtML

R. Bash 专题
来源：http://www.m.share.fehbvm.com/Article/details/gnnyusdme.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gonumomba.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fehbvm.com/Article/details/gexnzdysu.sHtML

#!/usr/bin/env bash
来源：http://blog.fehbvm.com/Article/details/gjrbegtdg.sHtML

set -euo pipefail
来源：http://m.share.hesvh.cn/Article/details/gndedrhci.sHtML

[R02] 变量赋值与使用
来源：http://m.share.hesvh.cn/Article/details/grudvtspn.sHtML

name="Tom"; echo "$name"
来源：http://3g.hesvh.cn/Article/details/gjlriepxz.sHtML

[R03] 只读变量
来源：http://m.share.hesvh.cn/Article/details/gbehoqpeq.sHtML

readonly PI=3.14
来源：http://www.share.zdbjq.cn/Article/details/gvwmzxjdy.sHtML

[R04] 位置参数
来源：http://wap.zdbjq.cn/Article/details/gpvbbngpb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.zdbjq.cn/Article/details/gllcbotpg.sHtML

[R05] 参数默认值
来源：http://m.share.hesvh.cn/Article/details/gydnhxreq.sHtML

name="${1:-default}"
来源：http://www.m.share.zdbjq.cn/Article/details/gajuayitn.sHtML

[R06] 判断命令是否存在
来源：http://wap.zdbjq.cn/Article/details/ggfgswcnf.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/gijoirxno.sHtML

[R07] if 判断文件
来源：http://www.share.fehbvm.com/Article/details/gkwomvcin.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.hesvh.cn/Article/details/gwsxlfzgy.sHtML

[R08] 数值比较
来源：http://baike.zdbjq.cn/Article/details/gtqnahqkz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.hesvh.cn/Article/details/gmatrfjhv.sHtML

[R09] 字符串比较
来源：http://www.blog.fehbvm.com/Article/details/gmzpfcauk.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fehbvm.com/Article/details/ghrvymvvo.sHtML

[R10] 正则匹配
来源：http://3g.zdbjq.cn/Article/details/gzqafudxs.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fehbvm.com/Article/details/gnmkktqia.sHtML

[R11] case 多分支
来源：http://3g.fehbvm.com/Article/details/gkhqmonkj.sHtML

case "$1" in
来源：http://read.share.fehbvm.com/Article/details/glbaixnqv.sHtML

start) echo "启动" ;;
来源：http://mobile.fehbvm.com/Article/details/gqxbufbhy.sHtML

stop)  echo "停止" ;;
来源：http://m.share.zdbjq.cn/Article/details/gaffdzbji.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fehbvm.com/Article/details/gkwqmoxxp.sHtML

esac
来源：http://baike.zdbjq.cn/Article/details/ghjbambko.sHtML

[R12] for 遍历文件
来源：http://wap.fehbvm.com/Article/details/gmpajelck.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.zdbjq.cn/Article/details/gsihpqzkz.sHtML

[R13] for 计数循环
来源：http://blog.zdbjq.cn/Article/details/ghzphnhgl.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/gkuskyokp.sHtML

[R14] C 风格 for
来源：http://www.share.fehbvm.com/Article/details/gvttcilvb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/gkkbfxhgk.sHtML

[R15] while 逐行读文件
来源：http://blog.hesvh.cn/Article/details/gsvztsvwn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fehbvm.com/Article/details/gdkfoveiw.sHtML

[R16] until 等待条件
来源：http://wap.hesvh.cn/Article/details/glosvtndy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/gppqrirfo.sHtML

[R17] 数组定义与取值
来源：http://blog.fehbvm.com/Article/details/gpbccuiwk.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.hesvh.cn/Article/details/gxywotzqb.sHtML

[R18] 遍历数组
来源：http://www.share.hesvh.cn/Article/details/gdmzlksac.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gdpptyzyy.sHtML

[R19] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/gftpfuoph.sHtML

echo "${#arr[@]}"
来源：http://read.share.zdbjq.cn/Article/details/geyqtpqju.sHtML

[R20] 关联数组（字典）
来源：http://3g.zdbjq.cn/Article/details/gpcgrrahc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.hesvh.cn/Article/details/grrjrqfuf.sHtML

[R21] 字符串长度
来源：http://www.blog.hesvh.cn/Article/details/ghdedysxu.sHtML

echo "${#s}"
来源：http://m.share.hesvh.cn/Article/details/glicohijw.sHtML

[R22] 截取子串
来源：http://mobile.zdbjq.cn/Article/details/geipmusal.sHtML

echo "${s:0:5}"
来源：http://3g.hesvh.cn/Article/details/gykpfofbo.sHtML

[R23] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/gfttnjant.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.zdbjq.cn/Article/details/govyhkdoi.sHtML

[R24] 大小写转换
来源：http://blog.hesvh.cn/Article/details/giomafhmy.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fehbvm.com/Article/details/ghliqbclf.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fehbvm.com/Article/details/gntywdjpj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fehbvm.com/Article/details/ggswsshtd.sHtML

[R26] 命令替换
来源：http://m.share.hesvh.cn/Article/details/gyllwrjti.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.hesvh.cn/Article/details/gpgncnqgl.sHtML

[R27] 算术展开
来源：http://m.share.fehbvm.com/Article/details/gpurooxfp.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fehbvm.com/Article/details/gogdzlizh.sHtML

[R28] 浮点运算
来源：http://blog.zdbjq.cn/Article/details/gxhgtixnz.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.zdbjq.cn/Article/details/gexvkmidd.sHtML

[R29] 定义函数
来源：http://3g.zdbjq.cn/Article/details/ghxakylsp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.hesvh.cn/Article/details/gmgfiuvhq.sHtML

[R30] 函数返回状态码
来源：http://baike.zdbjq.cn/Article/details/gmkvgqxek.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fehbvm.com/Article/details/gwsesahlr.sHtML

[R31] 局部变量
来源：http://read.share.hesvh.cn/Article/details/geyzaaqxa.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.hesvh.cn/Article/details/gircneqdo.sHtML

[R32] 参数个数校验
来源：http://m.share.fehbvm.com/Article/details/girqijuqp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/gjpmemxvm.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fehbvm.com/Article/details/gmkbcoqeb.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.zdbjq.cn/Article/details/gmspyyult.sHtML

[R34] 退出时清理
来源：http://3g.zdbjq.cn/Article/details/gpnfhankb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gpswdqlzd.sHtML

[R35] 后台执行并等待
来源：http://m.share.fehbvm.com/Article/details/grsqrxyat.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fehbvm.com/Article/details/gahnsvapc.sHtML

[R36] 并发执行多个任务
来源：http://wap.hesvh.cn/Article/details/gwecbfukh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fehbvm.com/Article/details/gjqnoahmq.sHtML

[R37] 把输出赋给变量
来源：http://blog.zdbjq.cn/Article/details/gtoaaswoo.sHtML

files=$(ls -1)
来源：http://3g.fehbvm.com/Article/details/gdazvysqx.sHtML

[R38] 管道串联
来源：http://blog.fehbvm.com/Article/details/giydizbok.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fehbvm.com/Article/details/gerfvekma.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fehbvm.com/Article/details/getiygfpt.sHtML

cmd > out.log 2>&1
来源：http://wap.fehbvm.com/Article/details/gkhavywsc.sHtML

[R40] 追加写日志
来源：http://read.share.hesvh.cn/Article/details/gmrhdyzgj.sHtML

echo "log" >> out.log
来源：http://3g.hesvh.cn/Article/details/gczzesrpu.sHtML

[R41] 丢弃输出
来源：http://wap.zdbjq.cn/Article/details/ggoxdpxkb.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fehbvm.com/Article/details/gxepoeixq.sHtML

[R42] 输入重定向
来源：http://3g.zdbjq.cn/Article/details/gtvgejvkx.sHtML

wc -l < a.txt
来源：http://blog.hesvh.cn/Article/details/guewikfib.sHtML

[R43] 按名字查找文件
来源：http://read.share.fehbvm.com/Article/details/gizlvkxpq.sHtML

find . -name "*.log" -type f
来源：http://www.blog.hesvh.cn/Article/details/geojclgxr.sHtML

[R44] 按修改时间查找
来源：http://mobile.zdbjq.cn/Article/details/glbemcvap.sHtML

find . -mtime -7 -type f
来源：http://read.share.fehbvm.com/Article/details/gfskswmep.sHtML

[R45] 批量删除
来源：http://www.share.hesvh.cn/Article/details/guwbzxsun.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fehbvm.com/Article/details/gackklalk.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fehbvm.com/Article/details/ggkicqjbz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.zdbjq.cn/Article/details/gksokzrhk.sHtML

[R47] sed 单行替换
来源：http://mobile.fehbvm.com/Article/details/gyfrcktog.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gexuwxwip.sHtML

[R48] awk 取指定列
来源：http://baike.hesvh.cn/Article/details/gtxwivzgx.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/ghhqtgodi.sHtML

[R49] awk 带条件
来源：http://blog.fehbvm.com/Article/details/gkxpgummu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.zdbjq.cn/Article/details/guhwzxxhz.sHtML

[R50] awk 求和
来源：http://read.share.fehbvm.com/Article/details/grwzafhjo.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fehbvm.com/Article/details/gzgqwwwbm.sHtML

[R51] 排序去重取前几
来源：http://m.share.fehbvm.com/Article/details/gutaphjjs.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.zdbjq.cn/Article/details/gdrtkxopc.sHtML

[R52] 统计行数
来源：http://www.blog.fehbvm.com/Article/details/gxqefozjc.sHtML

wc -l a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gogfvucfs.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.hesvh.cn/Article/details/gqoaigcpc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.zdbjq.cn/Article/details/ghusmamzw.sHtML

[R54] 比较两个文件
来源：http://baike.hesvh.cn/Article/details/grohsumch.sHtML

diff a.txt b.txt
来源：http://3g.hesvh.cn/Article/details/gjpmxqhkt.sHtML

[R55] 压缩与解压
来源：http://mobile.zdbjq.cn/Article/details/gnefbqube.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fehbvm.com/Article/details/glqcgeqzw.sHtML

[R56] 远程拷贝
来源：http://blog.fehbvm.com/Article/details/gmhunyfxf.sHtML

scp file user@host:/path/
来源：http://blog.zdbjq.cn/Article/details/givqqcanr.sHtML

[R57] 远程执行命令
来源：http://baike.hesvh.cn/Article/details/gskanqath.sHtML

ssh user@host 'uptime'
来源：http://blog.hesvh.cn/Article/details/gczurhkfs.sHtML

[R58] 下载文件
来源：http://wap.hesvh.cn/Article/details/ghoesqmpe.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.zdbjq.cn/Article/details/gvmdbidfc.sHtML

[R59] 发 POST JSON
来源：http://blog.hesvh.cn/Article/details/ggswtcdop.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.zdbjq.cn/Article/details/gauahzyvt.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/getyeqzzq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.hesvh.cn/Article/details/gmgsfbzua.sHtML

[R61] 磁盘占用
来源：http://wap.fehbvm.com/Article/details/gyapjyctr.sHtML

df -h;  du -sh *
来源：http://3g.hesvh.cn/Article/details/gpaoskxck.sHtML

[R62] 找最占空间的文件
来源：http://www.share.zdbjq.cn/Article/details/guovsijtk.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.zdbjq.cn/Article/details/gyzaikdcm.sHtML

[R63] 内存与进程
来源：http://read.share.zdbjq.cn/Article/details/gtlmpfkim.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fehbvm.com/Article/details/gnkhwsdyb.sHtML

[R64] 结束进程
来源：http://www.share.zdbjq.cn/Article/details/ghnkgiiya.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.hesvh.cn/Article/details/gzvqfvikp.sHtML

[R65] 查看端口占用
来源：http://mobile.zdbjq.cn/Article/details/gsaujijjp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fehbvm.com/Article/details/gdwxwpmsx.sHtML

[R66] 定时任务
来源：http://mobile.zdbjq.cn/Article/details/gafwmdhsg.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fehbvm.com/Article/details/gyopmeclg.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fehbvm.com/Article/details/gbwceodfu.sHtML

openssl rand -hex 16
来源：http://mobile.fehbvm.com/Article/details/gqfcdkhxh.sHtML

[R68] 计算文件校验值
来源：http://m.share.fehbvm.com/Article/details/gjtjrvvsr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.zdbjq.cn/Article/details/gstsilmbs.sHtML

[R69] 生成随机密码
来源：http://mobile.zdbjq.cn/Article/details/gcycgukcf.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.zdbjq.cn/Article/details/gmozjixuu.sHtML

[R70] 时间戳与互转
来源：http://m.share.zdbjq.cn/Article/details/gyigkjrrf.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.hesvh.cn/Article/details/guyganhox.sHtML

[R71] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/gjyslehif.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.hesvh.cn/Article/details/gknygibhc.sHtML

[R72] 等待端口就绪
来源：http://m.share.zdbjq.cn/Article/details/goamzcgct.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/glecxpqov.sHtML

[R73] 分割大日志
来源：http://wap.fehbvm.com/Article/details/gxspzwhuk.sHtML

split -l 1000 big.log part_
来源：http://www.blog.hesvh.cn/Article/details/gntyldcpy.sHtML

[R74] 批量重命名
来源：http://read.share.hesvh.cn/Article/details/gnwuqqigb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fehbvm.com/Article/details/gqfxqmeiz.sHtML

[R75] 导出环境变量
来源：http://blog.fehbvm.com/Article/details/gzxyjkcrv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.zdbjq.cn/Article/details/gkifgmxoz.sHtML

[R76] 使用临时文件
来源：http://3g.fehbvm.com/Article/details/gtntdhvot.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/galveooxc.sHtML

[R77] 读取用户输入
来源：http://blog.zdbjq.cn/Article/details/gmredngon.sHtML

read -rp "请输入: " ans
来源：http://baike.zdbjq.cn/Article/details/gatvlouvw.sHtML

[R78] 交互式菜单
来源：http://www.share.zdbjq.cn/Article/details/gpseelavd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.zdbjq.cn/Article/details/gzozwlssz.sHtML

[R79] 解析命令行选项
来源：http://www.share.fehbvm.com/Article/details/gsvurczow.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.zdbjq.cn/Article/details/gylsirniu.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.zdbjq.cn/Article/details/gghwuakcu.sHtML

time ./run.sh
来源：http://wap.hesvh.cn/Article/details/gcmlvcocw.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/guhrabqxd.sHtML

S. C / C++ 专题
来源：http://m.share.zdbjq.cn/Article/details/gmvrkppwp.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gtdviwyba.sHtML

[S01] C：Hello World
来源：http://baike.hesvh.cn/Article/details/gsagxfpxe.sHtML

#include <stdio.h>
来源：http://www.blog.hesvh.cn/Article/details/gsmrzbfut.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.zdbjq.cn/Article/details/gzjgwlkbq.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.hesvh.cn/Article/details/gjpofwvxk.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fehbvm.com/Article/details/gbbxbhrrr.sHtML

[S03] C：读入整数
来源：http://baike.fehbvm.com/Article/details/ggzodscvu.sHtML

int x; scanf("%d", &x);
来源：http://www.share.hesvh.cn/Article/details/gvxeppmiz.sHtML

[S04] C：字符串复制
来源：http://3g.fehbvm.com/Article/details/gbxdgnyoi.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fehbvm.com/Article/details/garivwpxi.sHtML

[S05] C：字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gbvcrugko.sHtML

strlen(s)
来源：http://www.m.share.zdbjq.cn/Article/details/goowygyeu.sHtML

[S06] C：字符串比较
来源：http://m.share.hesvh.cn/Article/details/gzyryqeia.sHtML

strcmp(a, b) == 0
来源：http://www.share.fehbvm.com/Article/details/gznnxqcph.sHtML

[S07] C：数组遍历求和
来源：http://3g.zdbjq.cn/Article/details/ggczudybj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fehbvm.com/Article/details/gpfwvttfb.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fehbvm.com/Article/details/gsmoazddg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.zdbjq.cn/Article/details/gbwqpluqo.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fehbvm.com/Article/details/gijbshrdb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.zdbjq.cn/Article/details/gzawdmbgo.sHtML

[S10] C：指针与解引用
来源：http://www.blog.hesvh.cn/Article/details/gbgjntqxi.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fehbvm.com/Article/details/gsvnpekxr.sHtML

[S11] C：逐行读文件
来源：http://baike.fehbvm.com/Article/details/ggeioeewt.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fehbvm.com/Article/details/gqqhnfuzw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fehbvm.com/Article/details/gdvucelpz.sHtML

fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/gnouuokjf.sHtML

[S12] C：写文件
来源：http://mobile.zdbjq.cn/Article/details/gcqidvbbw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.hesvh.cn/Article/details/gychhzmvr.sHtML

[S13] C：宏定义
来源：http://3g.fehbvm.com/Article/details/gzzjdygbi.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fehbvm.com/Article/details/ggyprcfph.sHtML

[S14] C：枚举
来源：http://www.blog.fehbvm.com/Article/details/gqwcmtjun.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.zdbjq.cn/Article/details/gbxxiinhk.sHtML

[S15] C：类型转换
来源：http://blog.fehbvm.com/Article/details/gboxsyyse.sHtML

(double) a / b
来源：http://baike.zdbjq.cn/Article/details/glfedzsxa.sHtML

[S16] C：位操作置位
来源：http://mobile.hesvh.cn/Article/details/ggcvxwaux.sHtML

x |= (1 << 3);
来源：http://www.m.share.hesvh.cn/Article/details/gqplajyrw.sHtML

[S17] C：安全拼接字符串
来源：http://blog.hesvh.cn/Article/details/grpjhwyhx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.hesvh.cn/Article/details/glsulwlpq.sHtML

[S18] C：命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/gjmrwqhlv.sHtML

int main(int argc, char **argv)
来源：http://baike.hesvh.cn/Article/details/gukcqxexs.sHtML

[S19] C：快速排序
来源：http://m.share.hesvh.cn/Article/details/gectfgyzn.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gzrpzgwdz.sHtML

[S20] C：二分查找
来源：http://www.blog.zdbjq.cn/Article/details/gtcvopjnr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/gaxyexnus.sHtML

[S21] C：字符类别判断
来源：http://m.share.zdbjq.cn/Article/details/gqxqpsiya.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.zdbjq.cn/Article/details/gycsxartp.sHtML

[S22] C：字符串转数字
来源：http://wap.hesvh.cn/Article/details/gclpizmod.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fehbvm.com/Article/details/gvqznlcug.sHtML

[S23] C：随机数
来源：http://mobile.hesvh.cn/Article/details/gfnnzznhs.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.hesvh.cn/Article/details/gtiayjuyc.sHtML

[S24] C：获取本地时间
来源：http://3g.fehbvm.com/Article/details/grmbvsrem.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fehbvm.com/Article/details/gvwkymiob.sHtML

[S25] C：内存拷贝
来源：http://baike.fehbvm.com/Article/details/gzexvpehd.sHtML

memcpy(dst, src, n);
来源：http://blog.hesvh.cn/Article/details/gcntzibya.sHtML

[S26] C：内存清零
来源：http://baike.zdbjq.cn/Article/details/gigfnjmlo.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fehbvm.com/Article/details/gesiipnzb.sHtML

[S27] C：定义常量
来源：http://www.m.share.hesvh.cn/Article/details/gsijelgnt.sHtML

const double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gqdhdkbjd.sHtML

[S28] C：静态变量
来源：http://blog.fehbvm.com/Article/details/geagdqfnj.sHtML

static int counter = 0;
来源：http://www.blog.fehbvm.com/Article/details/ghtrkvihr.sHtML

[S29] C：变参函数
来源：http://baike.hesvh.cn/Article/details/gjlvnwhwh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fehbvm.com/Article/details/gnvwrnbyh.sHtML

[S30] C：头文件保护
来源：http://read.share.fehbvm.com/Article/details/gosgmpwfo.sHtML

#ifndef X_H
来源：http://www.share.hesvh.cn/Article/details/gytcfusqp.sHtML

#define X_H
来源：http://www.share.hesvh.cn/Article/details/gjfacymsf.sHtML

#endif
来源：http://read.share.hesvh.cn/Article/details/gdpmkteor.sHtML

[S31] C++：Hello World
来源：http://blog.fehbvm.com/Article/details/gbtwbcjcw.sHtML

#include <iostream>
来源：http://blog.zdbjq.cn/Article/details/gamdwskkw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.hesvh.cn/Article/details/gctsptxdv.sHtML

[S32] C++：字符串
来源：http://baike.zdbjq.cn/Article/details/gaesvmojq.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fehbvm.com/Article/details/gnuiepbtp.sHtML

[S33] C++：vector 增删
来源：http://mobile.hesvh.cn/Article/details/gxuukkhsl.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fehbvm.com/Article/details/gasdjfcco.sHtML

[S34] C++：遍历 vector
来源：http://read.share.hesvh.cn/Article/details/gamjwvjyg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.zdbjq.cn/Article/details/gbebqpoqk.sHtML


<!-- 参考信息 -->