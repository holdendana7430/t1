代发 wailian999

[Q63] 开启事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gcywtfacj.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fanxiaobao.xyz/Article/details/gqsprjvks.sHtML

[Q64] 提交事务
来源：http://baike.fanxiaobao.xyz/Article/details/ggggopein.sHtML

COMMIT;
来源：http://blog.fanxiaobao.xyz/Article/details/gtcjsxzel.sHtML

[Q65] 回滚事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gxgntnelo.sHtML

ROLLBACK;
来源：http://read.share.fanxiaobao.xyz/Article/details/givrbisvq.sHtML

[Q66] 行锁查询
来源：http://blog.fanxiaobao.xyz/Article/details/gsmujorot.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fanxiaobao.xyz/Article/details/gskpwqlou.sHtML

[Q67] 设置隔离级别
来源：http://blog.fanxiaobao.xyz/Article/details/gmcpbkkqs.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmwnajrl.sHtML

[Q68] 保存点
来源：http://www.share.fanxiaobao.xyz/Article/details/giehjvsqo.sHtML

SAVEPOINT sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/grqrxgudo.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwuzdkoo.sHtML

[Q69] 查看执行计划
来源：http://www.share.fanxiaobao.xyz/Article/details/gbhcnrkln.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkvhplacd.sHtML

[Q70] 更新统计信息
来源：http://www.share.fanxiaobao.xyz/Article/details/gyjsktksf.sHtML

ANALYZE TABLE users;
来源：http://blog.fanxiaobao.xyz/Article/details/gtgobctdb.sHtML

[Q71] 查看建表语句
来源：http://read.share.fanxiaobao.xyz/Article/details/gcpsbpbtd.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fanxiaobao.xyz/Article/details/gndvdkhmc.sHtML

[Q72] 查看索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gmxxwpbhp.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhhrmafc.sHtML

[Q73] 查看表状态
来源：http://mobile.fanxiaobao.xyz/Article/details/gyzuqfawy.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnvneebgj.sHtML

[Q74] 强制使用索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gdlhbhxif.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fanxiaobao.xyz/Article/details/ganvmbywd.sHtML

[Q75] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gjvfclspc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gkkwxdbgk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fanxiaobao.xyz/Article/details/gdudjalgb.sHtML

[Q76] 按天统计
来源：http://www.share.fanxiaobao.xyz/Article/details/gxevhfcan.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fanxiaobao.xyz/Article/details/gxqjgkaas.sHtML

[Q77] 时间加减
来源：http://mobile.fanxiaobao.xyz/Article/details/gnrutllqo.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fanxiaobao.xyz/Article/details/gnapuoolr.sHtML

[Q78] 当前时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gfitadrnv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fanxiaobao.xyz/Article/details/gmcewphld.sHtML

[Q79] 字符串拼接
来源：http://m.share.fanxiaobao.xyz/Article/details/gvdxozqxl.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fanxiaobao.xyz/Article/details/geclkdieo.sHtML

[Q80] 字符串截取
来源：http://wap.fanxiaobao.xyz/Article/details/gudgabjod.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gbamxswtg.sHtML

[Q81] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gdxfrwmuh.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/giysbutup.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfsiuihf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtmnwhagg.sHtML

[Q83] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gxfnqkdso.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyfnnslln.sHtML

[Q84] 去除首尾空格
来源：http://wap.fanxiaobao.xyz/Article/details/gcdfakwgm.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gixvwzgtb.sHtML

[Q85] 数值取整
来源：http://baike.fanxiaobao.xyz/Article/details/ghwwjekgm.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fanxiaobao.xyz/Article/details/gdglufxho.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fanxiaobao.xyz/Article/details/gbvdwywwz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnovoqawq.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fanxiaobao.xyz/Article/details/gwfoluzdx.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grlmzvuaj.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fanxiaobao.xyz/Article/details/gxtvfadye.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqwpuckut.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmrpuzzqb.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gadqwumrq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngoipoti.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gawgflwme.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxcshjio.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gwqmvndrc.sHtML

R. Bash 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gsovppbgl.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gfppujqym.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fanxiaobao.xyz/Article/details/gzofxrapk.sHtML

#!/usr/bin/env bash
来源：http://www.share.fanxiaobao.xyz/Article/details/gkrtnqfau.sHtML

set -euo pipefail
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjibhfsd.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fanxiaobao.xyz/Article/details/geswlkqgp.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fanxiaobao.xyz/Article/details/grustkzvp.sHtML

[R03] 只读变量
来源：http://blog.fanxiaobao.xyz/Article/details/gxovvessm.sHtML

readonly PI=3.14
来源：http://baike.fanxiaobao.xyz/Article/details/gjrvhzdnh.sHtML

[R04] 位置参数
来源：http://m.share.fanxiaobao.xyz/Article/details/goosfypgg.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gikrktigx.sHtML

[R05] 参数默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/ggmyoqpbs.sHtML

name="${1:-default}"
来源：http://baike.fanxiaobao.xyz/Article/details/gkaljgrgf.sHtML

[R06] 判断命令是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gagnskscl.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghapaslvm.sHtML

[R07] if 判断文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gfhsczvum.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmquktcvx.sHtML

[R08] 数值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdamgrsb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwhddphu.sHtML

[R09] 字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/glpmbiotb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gpdgmdbch.sHtML

[R10] 正则匹配
来源：http://wap.fanxiaobao.xyz/Article/details/ggzxqwtyt.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gzfppkqou.sHtML

[R11] case 多分支
来源：http://3g.fanxiaobao.xyz/Article/details/geomrufkt.sHtML

case "$1" in
来源：http://mobile.fanxiaobao.xyz/Article/details/gchljaqbp.sHtML

start) echo "启动" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gyyylyufz.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gcmupawvj.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfnwojvgw.sHtML

esac
来源：http://m.share.fanxiaobao.xyz/Article/details/gbffgcfft.sHtML

[R12] for 遍历文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gfwnescgk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gfdxncokv.sHtML

[R13] for 计数循环
来源：http://blog.fanxiaobao.xyz/Article/details/gfnysxzmj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gnjspyrmc.sHtML

[R14] C 风格 for
来源：http://blog.fanxiaobao.xyz/Article/details/gkshnjpxb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/ghlbvieff.sHtML

[R15] while 逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gbtzyivbq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gnfknsrev.sHtML

[R16] until 等待条件
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzcsitim.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gococzinh.sHtML

[R17] 数组定义与取值
来源：http://blog.fanxiaobao.xyz/Article/details/giupgcjls.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gurgktzvi.sHtML

[R18] 遍历数组
来源：http://wap.fanxiaobao.xyz/Article/details/gkztgmtxh.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmrakavpb.sHtML

[R19] 数组长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gdikoxhix.sHtML

echo "${#arr[@]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/glfjtpits.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxxoecxw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gqqzxlbpg.sHtML

[R21] 字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gnbjuckvx.sHtML

echo "${#s}"
来源：http://wap.fanxiaobao.xyz/Article/details/gffnsrhho.sHtML

[R22] 截取子串
来源：http://www.share.fanxiaobao.xyz/Article/details/gfdynhtfp.sHtML

echo "${s:0:5}"
来源：http://mobile.fanxiaobao.xyz/Article/details/guywmfqgj.sHtML

[R23] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gqtdoaitx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gojztirkh.sHtML

[R24] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gwudhuxrb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fanxiaobao.xyz/Article/details/gpyexzqid.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdhyjogal.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fanxiaobao.xyz/Article/details/gbfekpvxg.sHtML

[R26] 命令替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gmtxlkixo.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fanxiaobao.xyz/Article/details/gvhoknzub.sHtML

[R27] 算术展开
来源：http://m.share.fanxiaobao.xyz/Article/details/gwamrpush.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvpaxfuz.sHtML

[R28] 浮点运算
来源：http://blog.fanxiaobao.xyz/Article/details/ggrijdwmi.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fanxiaobao.xyz/Article/details/gjolwbkfg.sHtML

[R29] 定义函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gecknjllu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fanxiaobao.xyz/Article/details/gwllplrnu.sHtML

[R30] 函数返回状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gwuwfxsui.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fanxiaobao.xyz/Article/details/guzkarjdx.sHtML

[R31] 局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gulvedijn.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fanxiaobao.xyz/Article/details/glrvsfxwk.sHtML

[R32] 参数个数校验
来源：http://baike.fanxiaobao.xyz/Article/details/gxcwppfob.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gzrtzgoda.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gifjuzsqp.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fanxiaobao.xyz/Article/details/gwhfudrig.sHtML

[R34] 退出时清理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gclsjhtrc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gfuruwiio.sHtML

[R35] 后台执行并等待
来源：http://3g.fanxiaobao.xyz/Article/details/ghzvtowoa.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbqxiedc.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvyaxpsnk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fanxiaobao.xyz/Article/details/gpkczwrwe.sHtML

[R37] 把输出赋给变量
来源：http://wap.fanxiaobao.xyz/Article/details/giprvpflo.sHtML

files=$(ls -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwxfuyqfh.sHtML

[R38] 管道串联
来源：http://baike.fanxiaobao.xyz/Article/details/gzzufyfzq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fanxiaobao.xyz/Article/details/gcrqshrtb.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gfcsgnyec.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gjjgykfmy.sHtML

[R40] 追加写日志
来源：http://3g.fanxiaobao.xyz/Article/details/gtvnzolaj.sHtML

echo "log" >> out.log
来源：http://baike.fanxiaobao.xyz/Article/details/gkeqqvzws.sHtML

[R41] 丢弃输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqarhgbyd.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gbnjmemcj.sHtML

[R42] 输入重定向
来源：http://baike.fanxiaobao.xyz/Article/details/gvglgfrly.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/ggrwlxocb.sHtML

[R43] 按名字查找文件
来源：http://3g.fanxiaobao.xyz/Article/details/gdydspadd.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpqqlyoae.sHtML

[R44] 按修改时间查找
来源：http://wap.fanxiaobao.xyz/Article/details/ggouxiumh.sHtML

find . -mtime -7 -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gyuvgzucp.sHtML

[R45] 批量删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gsszbylju.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnkgwjwzd.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fanxiaobao.xyz/Article/details/gztnnlyqo.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fanxiaobao.xyz/Article/details/givpdkknw.sHtML

[R47] sed 单行替换
来源：http://www.share.fanxiaobao.xyz/Article/details/ghsnrzeuk.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsuofmjms.sHtML

[R48] awk 取指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxsrlbksh.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzbihxihs.sHtML

[R49] awk 带条件
来源：http://blog.fanxiaobao.xyz/Article/details/gwrntazbf.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/gkxwtghlr.sHtML

[R50] awk 求和
来源：http://3g.fanxiaobao.xyz/Article/details/gtojnmval.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gisfmmsjw.sHtML

[R51] 排序去重取前几
来源：http://baike.fanxiaobao.xyz/Article/details/glqaliuvj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fanxiaobao.xyz/Article/details/gfhojlakj.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/gcqqbqkcw.sHtML

wc -l a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyppylodu.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhpixowh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fanxiaobao.xyz/Article/details/gfvfxyrol.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gppaubbxd.sHtML

diff a.txt b.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmytivcqc.sHtML

[R55] 压缩与解压
来源：http://wap.fanxiaobao.xyz/Article/details/gkbbmexok.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fanxiaobao.xyz/Article/details/gpgdqpwmz.sHtML

[R56] 远程拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gruybwwre.sHtML

scp file user@host:/path/
来源：http://blog.fanxiaobao.xyz/Article/details/ggoxcluiz.sHtML

[R57] 远程执行命令
来源：http://mobile.fanxiaobao.xyz/Article/details/giolwgpwv.sHtML

ssh user@host 'uptime'
来源：http://3g.fanxiaobao.xyz/Article/details/gzizmrqfy.sHtML

[R58] 下载文件
来源：http://baike.fanxiaobao.xyz/Article/details/goivsqxfi.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaavtvtej.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqmbaykvc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fanxiaobao.xyz/Article/details/guinqmofq.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/goetdiwzq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkutifle.sHtML

[R61] 磁盘占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gpujyyobj.sHtML

df -h;  du -sh *
来源：http://read.share.fanxiaobao.xyz/Article/details/gjcdljjkj.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gytbutauc.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fanxiaobao.xyz/Article/details/gvixouwdf.sHtML

[R63] 内存与进程
来源：http://wap.fanxiaobao.xyz/Article/details/geltmougf.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fanxiaobao.xyz/Article/details/gsojbofjg.sHtML

[R64] 结束进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gumvmijta.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmknqcoaz.sHtML

[R65] 查看端口占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gidhgtviw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fanxiaobao.xyz/Article/details/giflfbtif.sHtML

[R66] 定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwqodmxj.sHtML

crontab -e;  crontab -l
来源：http://m.share.fanxiaobao.xyz/Article/details/grorzgfvz.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fanxiaobao.xyz/Article/details/gpwnbgiff.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/gsuoharra.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwgybrnys.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggkfnpwge.sHtML

[R69] 生成随机密码
来源：http://baike.fanxiaobao.xyz/Article/details/gbcyvvwet.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fanxiaobao.xyz/Article/details/gitrckeax.sHtML

[R70] 时间戳与互转
来源：http://m.share.fanxiaobao.xyz/Article/details/gxspimqpl.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwlfpuft.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gowzuwovv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fanxiaobao.xyz/Article/details/gorrtdbzw.sHtML

[R72] 等待端口就绪
来源：http://read.share.fanxiaobao.xyz/Article/details/gnhlmhjkl.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gdzxmgnul.sHtML

[R73] 分割大日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gqqzsmryv.sHtML

split -l 1000 big.log part_
来源：http://blog.fanxiaobao.xyz/Article/details/gttbanzkc.sHtML

[R74] 批量重命名
来源：http://3g.fanxiaobao.xyz/Article/details/gwtewxtav.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gwjrczxwy.sHtML

[R75] 导出环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdvtjvium.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fanxiaobao.xyz/Article/details/gnelvkpdi.sHtML

[R76] 使用临时文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjfrbpzjg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gflofqhog.sHtML

[R77] 读取用户输入
来源：http://m.share.fanxiaobao.xyz/Article/details/gqaxajikr.sHtML

read -rp "请输入: " ans
来源：http://mobile.fanxiaobao.xyz/Article/details/godszjrmj.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/gfxeksouj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxnbfuprv.sHtML

[R79] 解析命令行选项
来源：http://m.share.fanxiaobao.xyz/Article/details/gvnnoogkl.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjpcffydy.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fanxiaobao.xyz/Article/details/gjiyjwqes.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/gynrmkezg.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfegsfki.sHtML

S. C / C++ 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gpqhgmwvh.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gyazjhgvx.sHtML

[S01] C：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/geumminbd.sHtML

#include <stdio.h>
来源：http://m.share.fanxiaobao.xyz/Article/details/gtlbhawjr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gebslysqu.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gqtgdvdtt.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/gppjudfbv.sHtML

[S03] C：读入整数
来源：http://read.share.fanxiaobao.xyz/Article/details/grsnfhvvz.sHtML

int x; scanf("%d", &x);
来源：http://wap.fanxiaobao.xyz/Article/details/gcqrmkuoh.sHtML

[S04] C：字符串复制
来源：http://baike.fanxiaobao.xyz/Article/details/gsrbbutvy.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/ghflcduca.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvxnamvz.sHtML

strlen(s)
来源：http://wap.fanxiaobao.xyz/Article/details/grhevrmzd.sHtML

[S06] C：字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gbqjygoyq.sHtML

strcmp(a, b) == 0
来源：http://read.share.fanxiaobao.xyz/Article/details/gzskelidq.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/gadyisynv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fanxiaobao.xyz/Article/details/giefiuuxi.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvzimrmg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fanxiaobao.xyz/Article/details/gglwpwvrg.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fanxiaobao.xyz/Article/details/gjqijkjhz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fanxiaobao.xyz/Article/details/guukumeok.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbkgrmfqx.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gphmxnsif.sHtML

[S11] C：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/grfqidhea.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gphinxdgj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmaicayap.sHtML

fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkytvgti.sHtML

[S12] C：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gwrkmppie.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glmgtkybr.sHtML

[S13] C：宏定义
来源：http://wap.fanxiaobao.xyz/Article/details/gkkovanrd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fanxiaobao.xyz/Article/details/gyagyrhas.sHtML

[S14] C：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gaoparhia.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fanxiaobao.xyz/Article/details/gokyidapq.sHtML

[S15] C：类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gyzhzlgmj.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/ggryddeam.sHtML

[S16] C：位操作置位
来源：http://m.share.fanxiaobao.xyz/Article/details/grdfrooqe.sHtML

x |= (1 << 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpuztkbrj.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/guorznmtm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fanxiaobao.xyz/Article/details/gchxdbigr.sHtML

[S18] C：命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gezsxhbch.sHtML

int main(int argc, char **argv)
来源：http://baike.fanxiaobao.xyz/Article/details/glslkgrkq.sHtML

[S19] C：快速排序
来源：http://3g.fanxiaobao.xyz/Article/details/gotpvfwym.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/guxzdkjml.sHtML

[S20] C：二分查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsrlbjkid.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/grdwhkvoj.sHtML

[S21] C：字符类别判断
来源：http://baike.fanxiaobao.xyz/Article/details/geikglqou.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fanxiaobao.xyz/Article/details/gwvqrjnsz.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/goxnkscmo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fanxiaobao.xyz/Article/details/gczsakkqy.sHtML

[S23] C：随机数
来源：http://m.share.fanxiaobao.xyz/Article/details/gaiglccia.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqpccezm.sHtML

[S24] C：获取本地时间
来源：http://baike.fanxiaobao.xyz/Article/details/griilbfmv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fanxiaobao.xyz/Article/details/gexuvzfub.sHtML

[S25] C：内存拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gaysqmdre.sHtML

memcpy(dst, src, n);
来源：http://baike.fanxiaobao.xyz/Article/details/gutnoobzk.sHtML

[S26] C：内存清零
来源：http://wap.fanxiaobao.xyz/Article/details/gpydlvbsk.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzaykoofy.sHtML

[S27] C：定义常量
来源：http://3g.fanxiaobao.xyz/Article/details/gfpkhxhyw.sHtML

const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gzvpeufqh.sHtML

[S28] C：静态变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gcztvbntm.sHtML

static int counter = 0;
来源：http://baike.fanxiaobao.xyz/Article/details/gbzewyrnw.sHtML

[S29] C：变参函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gwnkdyewf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fanxiaobao.xyz/Article/details/ghnfomdrk.sHtML

[S30] C：头文件保护
来源：http://3g.fanxiaobao.xyz/Article/details/gultxtgof.sHtML

#ifndef X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gtkubwqbl.sHtML

#define X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gkpfimgwa.sHtML

#endif
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkkzgmkbb.sHtML

[S31] C++：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gdpfzjfnb.sHtML

#include <iostream>
来源：http://3g.fanxiaobao.xyz/Article/details/gfzgyrgzp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmxzwshlb.sHtML

[S32] C++：字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gizwinhyi.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fanxiaobao.xyz/Article/details/grxrfquar.sHtML


<!-- 参考信息 -->