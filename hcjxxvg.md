代发 wailian999

[Q65] 回滚事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gfgfcywff.sHtML

ROLLBACK;
来源：http://www.blog.fanxiaobao.xyz/Article/details/guewlhosj.sHtML

[Q66] 行锁查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqpzgdmyk.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxsnrdpno.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcajcowaf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fanxiaobao.xyz/Article/details/grirjgqlq.sHtML

[Q68] 保存点
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geruzmjey.sHtML

SAVEPOINT sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gcyiyznfi.sHtML

ROLLBACK TO sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/gkwupiucb.sHtML

[Q69] 查看执行计划
来源：http://wap.fanxiaobao.xyz/Article/details/gjwbaacoy.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fanxiaobao.xyz/Article/details/grbuajlrd.sHtML

[Q70] 更新统计信息
来源：http://baike.fanxiaobao.xyz/Article/details/grbcwkmsa.sHtML

ANALYZE TABLE users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gskfusgnu.sHtML

[Q71] 查看建表语句
来源：http://www.share.fanxiaobao.xyz/Article/details/gwdpidatu.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.fanxiaobao.xyz/Article/details/gzjgecawe.sHtML

[Q72] 查看索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/goaxwombk.sHtML

SHOW INDEX FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gmfihrbmz.sHtML

[Q73] 查看表状态
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbfmazpg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gqrrkxeud.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gytkyilrw.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjvlcnyx.sHtML

[Q75] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gsaksdyua.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkdniwzku.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjrdnjym.sHtML

[Q76] 按天统计
来源：http://read.share.fanxiaobao.xyz/Article/details/gfnatager.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxixifql.sHtML

[Q77] 时间加减
来源：http://www.blog.fanxiaobao.xyz/Article/details/gewrasqcp.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.fanxiaobao.xyz/Article/details/gxdskanae.sHtML

[Q78] 当前时间
来源：http://read.share.fanxiaobao.xyz/Article/details/getuqnzsl.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fanxiaobao.xyz/Article/details/gdmahwapp.sHtML

[Q79] 字符串拼接
来源：http://blog.fanxiaobao.xyz/Article/details/gtmbrilqj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fanxiaobao.xyz/Article/details/gzjtgifoj.sHtML

[Q80] 字符串截取
来源：http://baike.fanxiaobao.xyz/Article/details/gaiknbvag.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gycogwzkm.sHtML

[Q81] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gpoobtceo.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gupxgmkuc.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fanxiaobao.xyz/Article/details/gzltuvcts.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/guegcepge.sHtML

[Q83] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpnkhzcqd.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gobzqkwhq.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fanxiaobao.xyz/Article/details/gcznlfyhi.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gaisgiumo.sHtML

[Q85] 数值取整
来源：http://m.share.fanxiaobao.xyz/Article/details/gxgmbibwf.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fanxiaobao.xyz/Article/details/gupzlghzi.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fanxiaobao.xyz/Article/details/gnuuhnunj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fanxiaobao.xyz/Article/details/glvhllunl.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fanxiaobao.xyz/Article/details/gjbqymzcp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fanxiaobao.xyz/Article/details/grrfeepdh.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fanxiaobao.xyz/Article/details/govrmkaws.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fanxiaobao.xyz/Article/details/gcqvytqfi.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvvmtlywj.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gcgzyrdoq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gimsugrcg.sHtML

[Q90] 生成序号列
来源：http://mobile.fanxiaobao.xyz/Article/details/gsumfwnck.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhzhsdtm.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gzyobefht.sHtML

R. Bash 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gnbckpnfa.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/ggegdxjvr.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggtmugofl.sHtML

#!/usr/bin/env bash
来源：http://baike.fanxiaobao.xyz/Article/details/gritrybqo.sHtML

set -euo pipefail
来源：http://3g.fanxiaobao.xyz/Article/details/gmmprdwys.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guqvufwlm.sHtML

name="Tom"; echo "$name"
来源：http://blog.fanxiaobao.xyz/Article/details/guowiazpq.sHtML

[R03] 只读变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmtjzced.sHtML

readonly PI=3.14
来源：http://mobile.fanxiaobao.xyz/Article/details/gcglmgyru.sHtML

[R04] 位置参数
来源：http://blog.fanxiaobao.xyz/Article/details/gljzftpbr.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fanxiaobao.xyz/Article/details/gzduhgmjw.sHtML

[R05] 参数默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/golwgqcig.sHtML

name="${1:-default}"
来源：http://blog.fanxiaobao.xyz/Article/details/gulqoqujt.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyyjepefj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhvlmvhm.sHtML

[R07] if 判断文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxpquyhr.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gexmsrdgw.sHtML

[R08] 数值比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxzduluby.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gowmmmcib.sHtML

[R09] 字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gcyipmacg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gynyhakjm.sHtML

[R10] 正则匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/ghydbjigx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gkgykpeyo.sHtML

[R11] case 多分支
来源：http://wap.fanxiaobao.xyz/Article/details/gwfonwoyf.sHtML

case "$1" in
来源：http://blog.fanxiaobao.xyz/Article/details/guwdjnkwo.sHtML

start) echo "启动" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gtjpowxzi.sHtML

stop)  echo "停止" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/grfrcpnmj.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbmragvqb.sHtML

esac
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghmfbxfvh.sHtML

[R12] for 遍历文件
来源：http://blog.fanxiaobao.xyz/Article/details/gvcdlyhhv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtzycgpmf.sHtML

[R13] for 计数循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gymaplmsy.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gzrqhzqng.sHtML

[R14] C 风格 for
来源：http://3g.fanxiaobao.xyz/Article/details/gyfohysxj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gszizpvwv.sHtML

[R15] while 逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gbunplgrq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gxddizbdz.sHtML

[R16] until 等待条件
来源：http://m.share.fanxiaobao.xyz/Article/details/grwrcjudn.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmzrfhlxg.sHtML

[R17] 数组定义与取值
来源：http://read.share.fanxiaobao.xyz/Article/details/gdtkdcvgd.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gottchrlj.sHtML

[R18] 遍历数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmayylkxf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcyzpiinz.sHtML

[R19] 数组长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gnywhkjwj.sHtML

echo "${#arr[@]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gcgovcwuf.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnoqqxgbc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gkcrzdkvv.sHtML

[R21] 字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gpaptnbyb.sHtML

echo "${#s}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gyduyxfxg.sHtML

[R22] 截取子串
来源：http://m.share.fanxiaobao.xyz/Article/details/gsyprcvex.sHtML

echo "${s:0:5}"
来源：http://blog.fanxiaobao.xyz/Article/details/ggppnyhna.sHtML

[R23] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtizqxngi.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glkjizbxt.sHtML

[R24] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gokmzhcmj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/ghekvwqmj.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/gebsonomu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjbscuqw.sHtML

[R26] 命令替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkkdzhjga.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fanxiaobao.xyz/Article/details/gclimnkkf.sHtML

[R27] 算术展开
来源：http://blog.fanxiaobao.xyz/Article/details/gtxexdztz.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fanxiaobao.xyz/Article/details/glfrpajvp.sHtML

[R28] 浮点运算
来源：http://mobile.fanxiaobao.xyz/Article/details/gppddaagt.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fanxiaobao.xyz/Article/details/gmdyistxf.sHtML

[R29] 定义函数
来源：http://blog.fanxiaobao.xyz/Article/details/gblpyppjt.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fanxiaobao.xyz/Article/details/guuegwacu.sHtML

[R30] 函数返回状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gxbahfvxc.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fanxiaobao.xyz/Article/details/glvlnhpfq.sHtML

[R31] 局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/gvekwzbne.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmmhutcnr.sHtML

[R32] 参数个数校验
来源：http://read.share.fanxiaobao.xyz/Article/details/gajozrxmf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gabsbxvyj.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fanxiaobao.xyz/Article/details/gmriosbhq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fanxiaobao.xyz/Article/details/gdcfqtmkp.sHtML

[R34] 退出时清理
来源：http://baike.fanxiaobao.xyz/Article/details/ggypjcpig.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gzgaekgiz.sHtML

[R35] 后台执行并等待
来源：http://www.share.fanxiaobao.xyz/Article/details/gppvttjyv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fanxiaobao.xyz/Article/details/gkeohoiuy.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gubsuidlv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/gnfayybch.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fanxiaobao.xyz/Article/details/goonjlxsh.sHtML

files=$(ls -1)
来源：http://wap.fanxiaobao.xyz/Article/details/gviahnypn.sHtML

[R38] 管道串联
来源：http://www.share.fanxiaobao.xyz/Article/details/gbijgysxw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbvhbqrxy.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fanxiaobao.xyz/Article/details/gvokvapaz.sHtML

cmd > out.log 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gyijebijm.sHtML

[R40] 追加写日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gpqxtzfco.sHtML

echo "log" >> out.log
来源：http://www.share.fanxiaobao.xyz/Article/details/grulwphzn.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/gnpmumrgp.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/glzazhtvi.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqlwykty.sHtML

wc -l < a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gqdybdwoo.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxryrrmeg.sHtML

find . -name "*.log" -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gzjhmzciw.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyqlhiqpf.sHtML

find . -mtime -7 -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gapgkpamp.sHtML

[R45] 批量删除
来源：http://www.share.fanxiaobao.xyz/Article/details/gjihwoznq.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fanxiaobao.xyz/Article/details/gckuxobmw.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbooocxs.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/gnbtrrbng.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gxgtcgnkx.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gqwthsfip.sHtML

[R48] awk 取指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/gjiouozxl.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gidjckqcg.sHtML

[R49] awk 带条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gujhzhbvr.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glcjdlybi.sHtML

[R50] awk 求和
来源：http://baike.fanxiaobao.xyz/Article/details/gfcknmchq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gpjfnjnfn.sHtML

[R51] 排序去重取前几
来源：http://3g.fanxiaobao.xyz/Article/details/gvosgvvey.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fanxiaobao.xyz/Article/details/glgwtiret.sHtML

[R52] 统计行数
来源：http://wap.fanxiaobao.xyz/Article/details/gviazbexr.sHtML

wc -l a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gzytckxgm.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fanxiaobao.xyz/Article/details/gcghzfgbd.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gkdqmnjli.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gxilbsxbv.sHtML

diff a.txt b.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtszzwjoe.sHtML

[R55] 压缩与解压
来源：http://mobile.fanxiaobao.xyz/Article/details/gzmixhufr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fanxiaobao.xyz/Article/details/gnhnswubg.sHtML

[R56] 远程拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gmejbxytd.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/gesttigrq.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzbaehjis.sHtML

ssh user@host 'uptime'
来源：http://3g.fanxiaobao.xyz/Article/details/gzhdastpp.sHtML

[R58] 下载文件
来源：http://3g.fanxiaobao.xyz/Article/details/gozjynrwt.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fanxiaobao.xyz/Article/details/gxyfakktw.sHtML

[R59] 发 POST JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gvaxyxgkx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gfiyvghph.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmlumrbl.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwlcguky.sHtML

[R61] 磁盘占用
来源：http://3g.fanxiaobao.xyz/Article/details/glwpygwlr.sHtML

df -h;  du -sh *
来源：http://m.share.fanxiaobao.xyz/Article/details/gkcfwjbcn.sHtML

[R62] 找最占空间的文件
来源：http://3g.fanxiaobao.xyz/Article/details/gipoavqit.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fanxiaobao.xyz/Article/details/gevkwwhny.sHtML

[R63] 内存与进程
来源：http://wap.fanxiaobao.xyz/Article/details/gbkpxqytr.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fanxiaobao.xyz/Article/details/gtyumklxt.sHtML

[R64] 结束进程
来源：http://3g.fanxiaobao.xyz/Article/details/gciarljnj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/gazkolufi.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwalhhzfs.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/gihudamwz.sHtML

[R66] 定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwsanvzs.sHtML

crontab -e;  crontab -l
来源：http://baike.fanxiaobao.xyz/Article/details/ghnohwuni.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fanxiaobao.xyz/Article/details/gqnbgauax.sHtML

openssl rand -hex 16
来源：http://baike.fanxiaobao.xyz/Article/details/gotiffqmk.sHtML

[R68] 计算文件校验值
来源：http://mobile.fanxiaobao.xyz/Article/details/gkiwrtmxr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gwnmuxnxl.sHtML

[R69] 生成随机密码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatcvytne.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fanxiaobao.xyz/Article/details/gaukgqpnp.sHtML

[R70] 时间戳与互转
来源：http://baike.fanxiaobao.xyz/Article/details/gekiyucnz.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fanxiaobao.xyz/Article/details/geczuoaju.sHtML

[R71] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/ggverfeiw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fanxiaobao.xyz/Article/details/gxynououe.sHtML

[R72] 等待端口就绪
来源：http://baike.fanxiaobao.xyz/Article/details/glliiacxj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gcaqhxclb.sHtML

[R73] 分割大日志
来源：http://blog.fanxiaobao.xyz/Article/details/gtstxukea.sHtML

split -l 1000 big.log part_
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkygmhke.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/gwhznhqyn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gmkimlmam.sHtML

[R75] 导出环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gcpqpbgjq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fanxiaobao.xyz/Article/details/gynibbbyb.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexxqozaq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjekgvaq.sHtML

[R77] 读取用户输入
来源：http://wap.fanxiaobao.xyz/Article/details/ggyenlvog.sHtML

read -rp "请输入: " ans
来源：http://wap.fanxiaobao.xyz/Article/details/gqsmhewzy.sHtML

[R78] 交互式菜单
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwspoxxln.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/glfpunuqr.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/gwvpxryvd.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fanxiaobao.xyz/Article/details/ghwpbnmyw.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/gfhrtgglx.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/gynmgyenf.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gbpzovvgc.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gspzvfqsx.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gzjwdpabc.sHtML

[S01] C：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gcjnnysrn.sHtML

#include <stdio.h>
来源：http://mobile.fanxiaobao.xyz/Article/details/guinfdhop.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnnqvdaky.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gdsujakng.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gixnclmpb.sHtML

[S03] C：读入整数
来源：http://wap.fanxiaobao.xyz/Article/details/gqiueszic.sHtML

int x; scanf("%d", &x);
来源：http://baike.fanxiaobao.xyz/Article/details/gkfcazjwt.sHtML

[S04] C：字符串复制
来源：http://wap.fanxiaobao.xyz/Article/details/gwhpuxfrt.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/glzzpiljf.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdzbipvgx.sHtML

strlen(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyeqyqzkl.sHtML

[S06] C：字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gllfwmqpx.sHtML

strcmp(a, b) == 0
来源：http://www.share.fanxiaobao.xyz/Article/details/gnpccngum.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gvfselaml.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fanxiaobao.xyz/Article/details/gdrhynczq.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fanxiaobao.xyz/Article/details/ggpahtjjg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fanxiaobao.xyz/Article/details/gmfqxxeed.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fanxiaobao.xyz/Article/details/gucatwxih.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbyzsaiul.sHtML

[S10] C：指针与解引用
来源：http://baike.fanxiaobao.xyz/Article/details/gxsvdjtjy.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gadamijtr.sHtML

[S11] C：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gubzimhnz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/gvybywwkz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gklazgnwz.sHtML

fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/giohlfuyv.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gnxqyrcca.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gquygadtj.sHtML

[S13] C：宏定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gamqvvikk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fanxiaobao.xyz/Article/details/gzxponitq.sHtML

[S14] C：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gekuumvfs.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fanxiaobao.xyz/Article/details/gsczkzewo.sHtML

[S15] C：类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gcjewcqre.sHtML

(double) a / b
来源：http://3g.fanxiaobao.xyz/Article/details/gtoenkwom.sHtML

[S16] C：位操作置位
来源：http://blog.fanxiaobao.xyz/Article/details/gakyaugmo.sHtML

x |= (1 << 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfgqvvruv.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxmwgvqi.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpckggcsp.sHtML

[S18] C：命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/gdzucgtcj.sHtML

int main(int argc, char **argv)
来源：http://3g.fanxiaobao.xyz/Article/details/gyswigijo.sHtML

[S19] C：快速排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqpmjmnjc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwgzuquss.sHtML

[S20] C：二分查找
来源：http://baike.fanxiaobao.xyz/Article/details/grkflqtqc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gzvjorcvq.sHtML

[S21] C：字符类别判断
来源：http://3g.fanxiaobao.xyz/Article/details/gemwkhrqt.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbefljqjs.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/ghfenpjzd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fanxiaobao.xyz/Article/details/gywmfuswg.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/gmenatehe.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxkbazlso.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grgwrdxjm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fanxiaobao.xyz/Article/details/gembhjecn.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxxllhvv.sHtML

memcpy(dst, src, n);
来源：http://blog.fanxiaobao.xyz/Article/details/gnqjfihxc.sHtML

[S26] C：内存清零
来源：http://www.blog.fanxiaobao.xyz/Article/details/gphdjfhqb.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtaanohqp.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/gtholdwop.sHtML

const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjcusxhdj.sHtML

[S28] C：静态变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gphyccsee.sHtML

static int counter = 0;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gckqwxlsy.sHtML

[S29] C：变参函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gajvoyxcb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjknedec.sHtML

[S30] C：头文件保护
来源：http://mobile.fanxiaobao.xyz/Article/details/gagnqiqgj.sHtML

#ifndef X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gbfabwpwy.sHtML

#define X_H
来源：http://baike.fanxiaobao.xyz/Article/details/ggdmhmdap.sHtML

#endif
来源：http://m.share.fanxiaobao.xyz/Article/details/gxnsyreic.sHtML

[S31] C++：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/ghlxsyktc.sHtML

#include <iostream>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvodzjomy.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvghorpnl.sHtML

[S32] C++：字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsekbbdmh.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fanxiaobao.xyz/Article/details/gpmlykrhh.sHtML

[S33] C++：vector 增删
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdjjrivf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejjjqszk.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqqhfycba.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/guavzsdjy.sHtML


<!-- 参考信息 -->