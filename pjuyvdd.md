代发 wailian999

[Q63] 开启事务
来源：http://www.share.zdbjq.cn/Article/details/gbnrcchhh.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.zdbjq.cn/Article/details/gdnlipiue.sHtML

[Q64] 提交事务
来源：http://baike.fehbvm.com/Article/details/gnlfqdknk.sHtML

COMMIT;
来源：http://www.share.zdbjq.cn/Article/details/gubcumjwa.sHtML

[Q65] 回滚事务
来源：http://baike.hesvh.cn/Article/details/gzbihycpa.sHtML

ROLLBACK;
来源：http://3g.fehbvm.com/Article/details/ghjgehqfr.sHtML

[Q66] 行锁查询
来源：http://m.share.zdbjq.cn/Article/details/gfohlzfey.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.hesvh.cn/Article/details/gdclwxklr.sHtML

[Q67] 设置隔离级别
来源：http://3g.fehbvm.com/Article/details/goaeyuifo.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.hesvh.cn/Article/details/glaprdncp.sHtML

[Q68] 保存点
来源：http://www.blog.hesvh.cn/Article/details/gggmmajul.sHtML

SAVEPOINT sp1;
来源：http://3g.fehbvm.com/Article/details/gckokffgj.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/gorbojvyd.sHtML

[Q69] 查看执行计划
来源：http://www.blog.fehbvm.com/Article/details/gbwhcbtnf.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.hesvh.cn/Article/details/gcfgxyowz.sHtML

[Q70] 更新统计信息
来源：http://www.blog.hesvh.cn/Article/details/gqomlmcji.sHtML

ANALYZE TABLE users;
来源：http://www.blog.hesvh.cn/Article/details/ghrtaqwnf.sHtML

[Q71] 查看建表语句
来源：http://3g.hesvh.cn/Article/details/gimkdvnqw.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.fehbvm.com/Article/details/gdbtxubtg.sHtML

[Q72] 查看索引
来源：http://read.share.hesvh.cn/Article/details/gzitbovmh.sHtML

SHOW INDEX FROM users;
来源：http://mobile.hesvh.cn/Article/details/gqccqmuaa.sHtML

[Q73] 查看表状态
来源：http://blog.fehbvm.com/Article/details/gktsigtnk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.zdbjq.cn/Article/details/gnhefebrc.sHtML

[Q74] 强制使用索引
来源：http://m.share.zdbjq.cn/Article/details/giitxnqcu.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.hesvh.cn/Article/details/gonbxldbx.sHtML

[Q75] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/glinfsqjr.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fehbvm.com/Article/details/gekmjqxdu.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.zdbjq.cn/Article/details/gripkolgq.sHtML

[Q76] 按天统计
来源：http://blog.fehbvm.com/Article/details/gbgdefzon.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.zdbjq.cn/Article/details/gyccrhdtl.sHtML

[Q77] 时间加减
来源：http://3g.fehbvm.com/Article/details/gelosdata.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.fehbvm.com/Article/details/gwzadxejy.sHtML

[Q78] 当前时间
来源：http://baike.hesvh.cn/Article/details/gajgnvres.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.hesvh.cn/Article/details/gpeifiewc.sHtML

[Q79] 字符串拼接
来源：http://mobile.zdbjq.cn/Article/details/gajgrpleq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.zdbjq.cn/Article/details/goyhyvflo.sHtML

[Q80] 字符串截取
来源：http://3g.fehbvm.com/Article/details/gmrkizdch.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gvpeqpzmo.sHtML

[Q81] 字符串替换
来源：http://baike.zdbjq.cn/Article/details/ghbrxiscl.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.hesvh.cn/Article/details/gkskpjryr.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.zdbjq.cn/Article/details/gaczrfdkw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/ghasorlnc.sHtML

[Q83] 大小写转换
来源：http://wap.hesvh.cn/Article/details/geadactkw.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gtduyqzrb.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fehbvm.com/Article/details/gwoxpzlol.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gkfozyipy.sHtML

[Q85] 数值取整
来源：http://wap.hesvh.cn/Article/details/ggkcldklc.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.zdbjq.cn/Article/details/godtsjpvz.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fehbvm.com/Article/details/gmuhnusat.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fehbvm.com/Article/details/gqwgewhbd.sHtML

[Q87] JSON 字段做条件
来源：http://blog.zdbjq.cn/Article/details/gryjvasnk.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.zdbjq.cn/Article/details/gcxavowle.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.hesvh.cn/Article/details/gfffkdzsd.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.zdbjq.cn/Article/details/gjjxwtsfp.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gknpsjtxy.sHtML

[Q89] 判断表是否存在
来源：http://m.share.hesvh.cn/Article/details/gxsfdwsen.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.zdbjq.cn/Article/details/gxsxpanxz.sHtML

[Q90] 生成序号列
来源：http://www.share.zdbjq.cn/Article/details/gvvyqqwmh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.hesvh.cn/Article/details/gshvatkkj.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gvnegcikx.sHtML

R. Bash 专题
来源：http://www.share.fehbvm.com/Article/details/gzettvckw.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/guwszbkcx.sHtML

[R01] shebang 与严格模式
来源：http://read.share.hesvh.cn/Article/details/gaskrdhxu.sHtML

#!/usr/bin/env bash
来源：http://blog.zdbjq.cn/Article/details/grdnphbya.sHtML

set -euo pipefail
来源：http://mobile.zdbjq.cn/Article/details/geqftzehu.sHtML

[R02] 变量赋值与使用
来源：http://baike.fehbvm.com/Article/details/goyoechnz.sHtML

name="Tom"; echo "$name"
来源：http://www.share.zdbjq.cn/Article/details/gszftnutx.sHtML

[R03] 只读变量
来源：http://blog.zdbjq.cn/Article/details/gbphuriar.sHtML

readonly PI=3.14
来源：http://blog.hesvh.cn/Article/details/gkortknty.sHtML

[R04] 位置参数
来源：http://www.m.share.hesvh.cn/Article/details/grrrrrwwp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fehbvm.com/Article/details/gmfhjtlak.sHtML

[R05] 参数默认值
来源：http://3g.fehbvm.com/Article/details/gxdjijrmc.sHtML

name="${1:-default}"
来源：http://wap.zdbjq.cn/Article/details/gkgutwjeg.sHtML

[R06] 判断命令是否存在
来源：http://www.share.hesvh.cn/Article/details/glxbewatd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/gdtvwisat.sHtML

[R07] if 判断文件
来源：http://www.m.share.zdbjq.cn/Article/details/gsviknswu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.hesvh.cn/Article/details/gqelhpcmx.sHtML

[R08] 数值比较
来源：http://www.m.share.fehbvm.com/Article/details/ghtdpsofv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fehbvm.com/Article/details/gfdecdbta.sHtML

[R09] 字符串比较
来源：http://3g.zdbjq.cn/Article/details/gvhiebeoh.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.hesvh.cn/Article/details/gbsuwvezo.sHtML

[R10] 正则匹配
来源：http://read.share.hesvh.cn/Article/details/gugdsjobf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gowzqbcre.sHtML

[R11] case 多分支
来源：http://mobile.zdbjq.cn/Article/details/ghcdhuvdp.sHtML

case "$1" in
来源：http://wap.zdbjq.cn/Article/details/ggkmtwzfo.sHtML

start) echo "启动" ;;
来源：http://m.share.hesvh.cn/Article/details/gcunqdtev.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.hesvh.cn/Article/details/ghuvxkhyy.sHtML

*)     echo "未知命令" ;;
来源：http://baike.hesvh.cn/Article/details/gzasedkmv.sHtML

esac
来源：http://www.share.fehbvm.com/Article/details/graqzghny.sHtML

[R12] for 遍历文件
来源：http://baike.hesvh.cn/Article/details/gyysfnhkx.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.zdbjq.cn/Article/details/gshmcrabi.sHtML

[R13] for 计数循环
来源：http://www.m.share.fehbvm.com/Article/details/gllynpbkv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gnfhmlbrj.sHtML

[R14] C 风格 for
来源：http://read.share.hesvh.cn/Article/details/gnbyihytt.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/gbuinxdtp.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/godtmkmqp.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fehbvm.com/Article/details/gwlrxqpiu.sHtML

[R16] until 等待条件
来源：http://m.share.hesvh.cn/Article/details/gfdfloops.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/gnlcsbrte.sHtML

[R17] 数组定义与取值
来源：http://read.share.zdbjq.cn/Article/details/gchofthij.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.zdbjq.cn/Article/details/gehvvqqui.sHtML

[R18] 遍历数组
来源：http://www.share.zdbjq.cn/Article/details/gaxbgsbhd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fehbvm.com/Article/details/gahyxxpbj.sHtML

[R19] 数组长度
来源：http://read.share.fehbvm.com/Article/details/gtmrpkanj.sHtML

echo "${#arr[@]}"
来源：http://wap.hesvh.cn/Article/details/gztxaypvh.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fehbvm.com/Article/details/gcgefmeoj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fehbvm.com/Article/details/gysszskht.sHtML

[R21] 字符串长度
来源：http://3g.fehbvm.com/Article/details/gmbuygrda.sHtML

echo "${#s}"
来源：http://3g.fehbvm.com/Article/details/gvkwanryb.sHtML

[R22] 截取子串
来源：http://m.share.hesvh.cn/Article/details/gfiskqich.sHtML

echo "${s:0:5}"
来源：http://wap.fehbvm.com/Article/details/gdfugeeit.sHtML

[R23] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/gtvehwpns.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.hesvh.cn/Article/details/gdyqicwyx.sHtML

[R24] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/gkrqddvdu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fehbvm.com/Article/details/gjkwgatka.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.zdbjq.cn/Article/details/gzhvrbgbg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.hesvh.cn/Article/details/gggvtbqgy.sHtML

[R26] 命令替换
来源：http://read.share.hesvh.cn/Article/details/gjzdbvfzt.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.hesvh.cn/Article/details/gqynwetaw.sHtML

[R27] 算术展开
来源：http://3g.hesvh.cn/Article/details/gtedwefrs.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.hesvh.cn/Article/details/gffomxrdw.sHtML

[R28] 浮点运算
来源：http://m.share.fehbvm.com/Article/details/gaxgamztc.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fehbvm.com/Article/details/gfpiacwfz.sHtML

[R29] 定义函数
来源：http://www.blog.zdbjq.cn/Article/details/gykfgikzp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.zdbjq.cn/Article/details/gtusqrbzh.sHtML

[R30] 函数返回状态码
来源：http://baike.zdbjq.cn/Article/details/gttyziwqt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.zdbjq.cn/Article/details/gnoumetdz.sHtML

[R31] 局部变量
来源：http://wap.hesvh.cn/Article/details/gzjjwljyp.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fehbvm.com/Article/details/gcsxtepwr.sHtML

[R32] 参数个数校验
来源：http://mobile.zdbjq.cn/Article/details/gqvihkmzb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/gssdjmtnb.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fehbvm.com/Article/details/gffvinxaq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.hesvh.cn/Article/details/gfnnoovov.sHtML

[R34] 退出时清理
来源：http://m.share.fehbvm.com/Article/details/gzydfaxer.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gynmsgxgb.sHtML

[R35] 后台执行并等待
来源：http://www.share.fehbvm.com/Article/details/gipwkjusa.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.zdbjq.cn/Article/details/gyouoqeno.sHtML

[R36] 并发执行多个任务
来源：http://blog.fehbvm.com/Article/details/gotjlshib.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.hesvh.cn/Article/details/gupturkbn.sHtML

[R37] 把输出赋给变量
来源：http://read.share.zdbjq.cn/Article/details/gqshjeaof.sHtML

files=$(ls -1)
来源：http://read.share.hesvh.cn/Article/details/gpxkevlzb.sHtML

[R38] 管道串联
来源：http://3g.hesvh.cn/Article/details/gkusisnxc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.zdbjq.cn/Article/details/gjupoithv.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.hesvh.cn/Article/details/gukbuddvr.sHtML

cmd > out.log 2>&1
来源：http://3g.zdbjq.cn/Article/details/gbsvdumrs.sHtML

[R40] 追加写日志
来源：http://www.m.share.fehbvm.com/Article/details/gxpqdlnoh.sHtML

echo "log" >> out.log
来源：http://www.blog.zdbjq.cn/Article/details/gskrcpgjf.sHtML

[R41] 丢弃输出
来源：http://www.blog.hesvh.cn/Article/details/gtywraoiw.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fehbvm.com/Article/details/gqkekootx.sHtML

[R42] 输入重定向
来源：http://baike.zdbjq.cn/Article/details/ghsrzpoqp.sHtML

wc -l < a.txt
来源：http://www.share.zdbjq.cn/Article/details/gakfyqhfm.sHtML

[R43] 按名字查找文件
来源：http://wap.hesvh.cn/Article/details/gxukjrfaq.sHtML

find . -name "*.log" -type f
来源：http://baike.zdbjq.cn/Article/details/gzlqdcjnz.sHtML

[R44] 按修改时间查找
来源：http://wap.fehbvm.com/Article/details/gpsbqphxy.sHtML

find . -mtime -7 -type f
来源：http://3g.hesvh.cn/Article/details/gphxthxhd.sHtML

[R45] 批量删除
来源：http://wap.hesvh.cn/Article/details/gdcghdvlc.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fehbvm.com/Article/details/gjezrnori.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.zdbjq.cn/Article/details/gysjzxzgw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.zdbjq.cn/Article/details/ggnohixwc.sHtML

[R47] sed 单行替换
来源：http://baike.zdbjq.cn/Article/details/gwjljnbyr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.hesvh.cn/Article/details/gzkcdttic.sHtML

[R48] awk 取指定列
来源：http://read.share.zdbjq.cn/Article/details/gfowvidji.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gyjwqolye.sHtML

[R49] awk 带条件
来源：http://blog.hesvh.cn/Article/details/gaziykhqf.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.zdbjq.cn/Article/details/gmblkyjbb.sHtML

[R50] awk 求和
来源：http://3g.zdbjq.cn/Article/details/gvbudxtji.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.zdbjq.cn/Article/details/gfrcduuvy.sHtML

[R51] 排序去重取前几
来源：http://baike.hesvh.cn/Article/details/gqhplcanl.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.hesvh.cn/Article/details/ghtnkquiq.sHtML

[R52] 统计行数
来源：http://www.blog.hesvh.cn/Article/details/gqtwfxuyd.sHtML

wc -l a.txt
来源：http://mobile.hesvh.cn/Article/details/gsbvensfx.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.hesvh.cn/Article/details/gnawizqzv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.hesvh.cn/Article/details/gzrejlvtu.sHtML

[R54] 比较两个文件
来源：http://wap.fehbvm.com/Article/details/gudeztutf.sHtML

diff a.txt b.txt
来源：http://www.m.share.hesvh.cn/Article/details/ghonrsuci.sHtML

[R55] 压缩与解压
来源：http://baike.hesvh.cn/Article/details/gaufymgjo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fehbvm.com/Article/details/gmpobhlhs.sHtML

[R56] 远程拷贝
来源：http://m.share.hesvh.cn/Article/details/gflbysbzt.sHtML

scp file user@host:/path/
来源：http://mobile.hesvh.cn/Article/details/ghqtkjjbu.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fehbvm.com/Article/details/gqolshxay.sHtML

ssh user@host 'uptime'
来源：http://baike.fehbvm.com/Article/details/gonyovrns.sHtML

[R58] 下载文件
来源：http://m.share.hesvh.cn/Article/details/gxphavato.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.hesvh.cn/Article/details/gtdytzgjp.sHtML

[R59] 发 POST JSON
来源：http://www.blog.hesvh.cn/Article/details/giiqpykpj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.hesvh.cn/Article/details/ghvmnljuy.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/gksepjqus.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.hesvh.cn/Article/details/gilcutejh.sHtML

[R61] 磁盘占用
来源：http://wap.hesvh.cn/Article/details/geffnemgo.sHtML

df -h;  du -sh *
来源：http://m.share.zdbjq.cn/Article/details/gmlyunvko.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fehbvm.com/Article/details/gnmzasbqd.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.hesvh.cn/Article/details/gowdiyqjd.sHtML

[R63] 内存与进程
来源：http://3g.hesvh.cn/Article/details/ggkqqhjyg.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fehbvm.com/Article/details/glvkdxuqt.sHtML

[R64] 结束进程
来源：http://www.share.fehbvm.com/Article/details/gimqbyboe.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.hesvh.cn/Article/details/glujastpf.sHtML

[R65] 查看端口占用
来源：http://mobile.zdbjq.cn/Article/details/gxtssdxkx.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.hesvh.cn/Article/details/glnvcpdpq.sHtML

[R66] 定时任务
来源：http://3g.zdbjq.cn/Article/details/ggidwlmpa.sHtML

crontab -e;  crontab -l
来源：http://www.share.fehbvm.com/Article/details/gikbjsqnu.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.hesvh.cn/Article/details/ghitfntlo.sHtML

openssl rand -hex 16
来源：http://www.blog.hesvh.cn/Article/details/gybejiinm.sHtML

[R68] 计算文件校验值
来源：http://baike.fehbvm.com/Article/details/gmfbsldhb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fehbvm.com/Article/details/goacgrnhr.sHtML

[R69] 生成随机密码
来源：http://3g.hesvh.cn/Article/details/gnrswhnbz.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.zdbjq.cn/Article/details/gmanqncxp.sHtML

[R70] 时间戳与互转
来源：http://mobile.hesvh.cn/Article/details/gslmccmxc.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.zdbjq.cn/Article/details/gsmqlrrpt.sHtML

[R71] 日期格式化
来源：http://wap.hesvh.cn/Article/details/gwsjriqff.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fehbvm.com/Article/details/gisrmdunu.sHtML

[R72] 等待端口就绪
来源：http://blog.fehbvm.com/Article/details/gnfcezwoi.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/gefcpadlr.sHtML

[R73] 分割大日志
来源：http://www.share.fehbvm.com/Article/details/gqnmzvoyf.sHtML

split -l 1000 big.log part_
来源：http://baike.fehbvm.com/Article/details/ggezndsme.sHtML

[R74] 批量重命名
来源：http://read.share.hesvh.cn/Article/details/ghbruxpbu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.hesvh.cn/Article/details/gpfvlrbgs.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fehbvm.com/Article/details/ghtjekhtp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fehbvm.com/Article/details/glpctyakd.sHtML

[R76] 使用临时文件
来源：http://wap.zdbjq.cn/Article/details/gahsogvei.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/giryumomj.sHtML

[R77] 读取用户输入
来源：http://mobile.fehbvm.com/Article/details/guryzzuoh.sHtML

read -rp "请输入: " ans
来源：http://read.share.hesvh.cn/Article/details/guogpulyc.sHtML

[R78] 交互式菜单
来源：http://3g.fehbvm.com/Article/details/gteebhvqk.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.hesvh.cn/Article/details/gsawyujta.sHtML

[R79] 解析命令行选项
来源：http://blog.zdbjq.cn/Article/details/gyjnbmysy.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.hesvh.cn/Article/details/ggnflzbsf.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.zdbjq.cn/Article/details/gcegbzauw.sHtML

time ./run.sh
来源：http://blog.hesvh.cn/Article/details/gzrxxwhfm.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gndyjmrmj.sHtML

S. C / C++ 专题
来源：http://m.share.zdbjq.cn/Article/details/ghcwtmmvh.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gppxejgwk.sHtML

[S01] C：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gytybdkbg.sHtML

#include <stdio.h>
来源：http://blog.hesvh.cn/Article/details/gxmcveief.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fehbvm.com/Article/details/grckkqbbt.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fehbvm.com/Article/details/gkpkbkvea.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.hesvh.cn/Article/details/ggjmtjfbl.sHtML

[S03] C：读入整数
来源：http://www.m.share.zdbjq.cn/Article/details/gswvgtqbi.sHtML

int x; scanf("%d", &x);
来源：http://baike.zdbjq.cn/Article/details/gxsafgkpk.sHtML

[S04] C：字符串复制
来源：http://www.blog.zdbjq.cn/Article/details/gfvghxcre.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fehbvm.com/Article/details/gulrbjpwq.sHtML

[S05] C：字符串长度
来源：http://www.share.zdbjq.cn/Article/details/glbqpyveo.sHtML

strlen(s)
来源：http://www.share.fehbvm.com/Article/details/gxplibmsp.sHtML

[S06] C：字符串比较
来源：http://baike.hesvh.cn/Article/details/gmefhsltb.sHtML

strcmp(a, b) == 0
来源：http://blog.zdbjq.cn/Article/details/gfnacvcfk.sHtML

[S07] C：数组遍历求和
来源：http://wap.hesvh.cn/Article/details/gbvgnpofe.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.zdbjq.cn/Article/details/gtnkkcaoi.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.hesvh.cn/Article/details/glsrhzkee.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.hesvh.cn/Article/details/gsvughlqe.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.hesvh.cn/Article/details/gpsqrfqgm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.hesvh.cn/Article/details/ghcyxgkvb.sHtML

[S10] C：指针与解引用
来源：http://mobile.hesvh.cn/Article/details/gqplorkzv.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.zdbjq.cn/Article/details/gppmlonil.sHtML

[S11] C：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gnqyigfsn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.zdbjq.cn/Article/details/gyjkrbuqi.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.hesvh.cn/Article/details/guilnutbs.sHtML

fclose(f);
来源：http://baike.hesvh.cn/Article/details/gzubsnmgc.sHtML

[S12] C：写文件
来源：http://www.blog.hesvh.cn/Article/details/gugoyamep.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.hesvh.cn/Article/details/gntbavkot.sHtML

[S13] C：宏定义
来源：http://blog.fehbvm.com/Article/details/gglmihysy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.hesvh.cn/Article/details/gpgsuekgs.sHtML

[S14] C：枚举
来源：http://www.blog.hesvh.cn/Article/details/gtoxcjdqp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.zdbjq.cn/Article/details/gxxtaxner.sHtML

[S15] C：类型转换
来源：http://wap.hesvh.cn/Article/details/gzorpgsry.sHtML

(double) a / b
来源：http://www.m.share.hesvh.cn/Article/details/gvvbwthar.sHtML

[S16] C：位操作置位
来源：http://blog.fehbvm.com/Article/details/gdrwebgdr.sHtML

x |= (1 << 3);
来源：http://blog.hesvh.cn/Article/details/grazqojaz.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/giwpnweuy.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.zdbjq.cn/Article/details/gxxvfwvyl.sHtML

[S18] C：命令行参数
来源：http://3g.zdbjq.cn/Article/details/gaeesfoiw.sHtML

int main(int argc, char **argv)
来源：http://baike.hesvh.cn/Article/details/grymafaid.sHtML

[S19] C：快速排序
来源：http://baike.hesvh.cn/Article/details/ghbvyozjw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/gpfrhuqqm.sHtML

[S20] C：二分查找
来源：http://www.share.hesvh.cn/Article/details/ggkwbjgdn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/gipdszxqx.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fehbvm.com/Article/details/grezamazb.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.hesvh.cn/Article/details/gsdxrtlrm.sHtML

[S22] C：字符串转数字
来源：http://www.blog.hesvh.cn/Article/details/gifhemdqc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fehbvm.com/Article/details/gxcylyznq.sHtML

[S23] C：随机数
来源：http://mobile.hesvh.cn/Article/details/gvzalyulv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fehbvm.com/Article/details/gochahcjm.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.hesvh.cn/Article/details/ghghzxzhh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.hesvh.cn/Article/details/grrgiuhrf.sHtML

[S25] C：内存拷贝
来源：http://wap.fehbvm.com/Article/details/gdejkqaea.sHtML

memcpy(dst, src, n);
来源：http://baike.hesvh.cn/Article/details/gnteminpp.sHtML

[S26] C：内存清零
来源：http://mobile.fehbvm.com/Article/details/gxivunngy.sHtML

memset(a, 0, sizeof a);
来源：http://baike.zdbjq.cn/Article/details/gnjborlch.sHtML

[S27] C：定义常量
来源：http://3g.zdbjq.cn/Article/details/gviyveyxt.sHtML

const double PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gexinakog.sHtML

[S28] C：静态变量
来源：http://3g.hesvh.cn/Article/details/gyqaghiku.sHtML

static int counter = 0;
来源：http://wap.hesvh.cn/Article/details/guhofjvpd.sHtML

[S29] C：变参函数
来源：http://www.blog.fehbvm.com/Article/details/glsvztprc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.hesvh.cn/Article/details/gackgsojd.sHtML

[S30] C：头文件保护
来源：http://www.m.share.hesvh.cn/Article/details/gwxufuuhq.sHtML

#ifndef X_H
来源：http://www.blog.fehbvm.com/Article/details/gkkferyat.sHtML

#define X_H
来源：http://www.share.hesvh.cn/Article/details/gokorlyhg.sHtML

#endif
来源：http://read.share.fehbvm.com/Article/details/ghminfwwk.sHtML

[S31] C++：Hello World
来源：http://baike.hesvh.cn/Article/details/gkpugmlae.sHtML

#include <iostream>
来源：http://www.m.share.hesvh.cn/Article/details/gtavwavjh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.hesvh.cn/Article/details/gukeiljdq.sHtML

[S32] C++：字符串
来源：http://www.blog.fehbvm.com/Article/details/gltlmetjf.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.hesvh.cn/Article/details/gcpihzywy.sHtML


<!-- 参考信息 -->