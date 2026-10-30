代发 wailian999

[Q63] 开启事务
来源：http://mobile.zdbjq.cn/Article/details/ghrdzgogt.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.zdbjq.cn/Article/details/gnmnfokax.sHtML

[Q64] 提交事务
来源：http://www.blog.fehbvm.com/Article/details/gylipyqhf.sHtML

COMMIT;
来源：http://read.share.zdbjq.cn/Article/details/gvsrjzjii.sHtML

[Q65] 回滚事务
来源：http://baike.hesvh.cn/Article/details/gmzojuqjo.sHtML

ROLLBACK;
来源：http://www.blog.fehbvm.com/Article/details/gqlzkztta.sHtML

[Q66] 行锁查询
来源：http://m.share.fehbvm.com/Article/details/gdawsnyri.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fehbvm.com/Article/details/grggcxjim.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.hesvh.cn/Article/details/grphmxbaj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.zdbjq.cn/Article/details/gogwhhfsk.sHtML

[Q68] 保存点
来源：http://3g.zdbjq.cn/Article/details/gvpbeqiny.sHtML

SAVEPOINT sp1;
来源：http://mobile.zdbjq.cn/Article/details/genljyojr.sHtML

ROLLBACK TO sp1;
来源：http://wap.fehbvm.com/Article/details/gimfklzms.sHtML

[Q69] 查看执行计划
来源：http://blog.zdbjq.cn/Article/details/gvqbcatcf.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.hesvh.cn/Article/details/ggeutobpf.sHtML

[Q70] 更新统计信息
来源：http://baike.fehbvm.com/Article/details/gsfaxepyh.sHtML

ANALYZE TABLE users;
来源：http://3g.zdbjq.cn/Article/details/gmehytilx.sHtML

[Q71] 查看建表语句
来源：http://www.share.zdbjq.cn/Article/details/gzqyhmqcq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fehbvm.com/Article/details/gqzdyzxey.sHtML

[Q72] 查看索引
来源：http://m.share.zdbjq.cn/Article/details/gkzzqdjqz.sHtML

SHOW INDEX FROM users;
来源：http://mobile.hesvh.cn/Article/details/gkbaminzj.sHtML

[Q73] 查看表状态
来源：http://read.share.hesvh.cn/Article/details/gsnahpouz.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.hesvh.cn/Article/details/gdtmpskno.sHtML

[Q74] 强制使用索引
来源：http://m.share.zdbjq.cn/Article/details/gfxnmxnsd.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fehbvm.com/Article/details/gbflscbpl.sHtML

[Q75] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/grdrdvrjm.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fehbvm.com/Article/details/galkgubtc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.hesvh.cn/Article/details/gtubljfhk.sHtML

[Q76] 按天统计
来源：http://www.share.hesvh.cn/Article/details/gajkxzcjo.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.hesvh.cn/Article/details/grayzwnio.sHtML

[Q77] 时间加减
来源：http://mobile.fehbvm.com/Article/details/gpkqnucza.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.hesvh.cn/Article/details/gagbpjupr.sHtML

[Q78] 当前时间
来源：http://wap.fehbvm.com/Article/details/ghzsekvxi.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.zdbjq.cn/Article/details/gdgbeokvl.sHtML

[Q79] 字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/gmbqvhoeh.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.hesvh.cn/Article/details/gokjnetst.sHtML

[Q80] 字符串截取
来源：http://www.share.fehbvm.com/Article/details/gfgicfxft.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.hesvh.cn/Article/details/gkwjdlvrr.sHtML

[Q81] 字符串替换
来源：http://wap.fehbvm.com/Article/details/gjmzlmjoc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gdnkyuwcs.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.zdbjq.cn/Article/details/gdkjqbnye.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gsepovwgg.sHtML

[Q83] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gllxkmtdo.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gyviecqje.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fehbvm.com/Article/details/grimunjil.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gpmqpspyn.sHtML

[Q85] 数值取整
来源：http://www.m.share.fehbvm.com/Article/details/gfpjfefor.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.zdbjq.cn/Article/details/gvzczgtew.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.zdbjq.cn/Article/details/grmfzisiz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.zdbjq.cn/Article/details/gknqmsfsc.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fehbvm.com/Article/details/gpokyudbe.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fehbvm.com/Article/details/gjhlgwkor.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.zdbjq.cn/Article/details/gmnovznqf.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.zdbjq.cn/Article/details/gnxjbmvit.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.hesvh.cn/Article/details/gcwsvwghg.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.zdbjq.cn/Article/details/ghlelaafe.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fehbvm.com/Article/details/gsfogokkd.sHtML

[Q90] 生成序号列
来源：http://3g.fehbvm.com/Article/details/gpycaipjk.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fehbvm.com/Article/details/gezxwyiyy.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/grpnbcxos.sHtML

R. Bash 专题
来源：http://blog.fehbvm.com/Article/details/groqwbvmz.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gogkoelly.sHtML

[R01] shebang 与严格模式
来源：http://baike.fehbvm.com/Article/details/gfxefgevk.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fehbvm.com/Article/details/gaocsybsg.sHtML

set -euo pipefail
来源：http://www.blog.fehbvm.com/Article/details/gswfmsdqk.sHtML

[R02] 变量赋值与使用
来源：http://blog.hesvh.cn/Article/details/gnqslfwwe.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fehbvm.com/Article/details/gzyhmspcb.sHtML

[R03] 只读变量
来源：http://wap.fehbvm.com/Article/details/gouglllpw.sHtML

readonly PI=3.14
来源：http://www.blog.hesvh.cn/Article/details/gmikltnwn.sHtML

[R04] 位置参数
来源：http://mobile.fehbvm.com/Article/details/goeimcpof.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fehbvm.com/Article/details/ghvydgkba.sHtML

[R05] 参数默认值
来源：http://www.m.share.fehbvm.com/Article/details/gwhlamtbe.sHtML

name="${1:-default}"
来源：http://mobile.hesvh.cn/Article/details/gdhjoueeo.sHtML

[R06] 判断命令是否存在
来源：http://read.share.zdbjq.cn/Article/details/gaxtrxgap.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/gbwcthcpv.sHtML

[R07] if 判断文件
来源：http://m.share.hesvh.cn/Article/details/gdprmfvdf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fehbvm.com/Article/details/ggbccinys.sHtML

[R08] 数值比较
来源：http://3g.fehbvm.com/Article/details/gghvqkrzd.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gtvpqucfd.sHtML

[R09] 字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gkgnistet.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gutargrpt.sHtML

[R10] 正则匹配
来源：http://3g.fehbvm.com/Article/details/gceoequnx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.hesvh.cn/Article/details/gdjpqsrkj.sHtML

[R11] case 多分支
来源：http://mobile.fehbvm.com/Article/details/gkpqngvml.sHtML

case "$1" in
来源：http://3g.fehbvm.com/Article/details/gxpdsrcck.sHtML

start) echo "启动" ;;
来源：http://www.share.fehbvm.com/Article/details/gebxjyvge.sHtML

stop)  echo "停止" ;;
来源：http://3g.hesvh.cn/Article/details/gzufratee.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.hesvh.cn/Article/details/gmupscegz.sHtML

esac
来源：http://read.share.hesvh.cn/Article/details/gdgftjzso.sHtML

[R12] for 遍历文件
来源：http://baike.zdbjq.cn/Article/details/gynpiuiqk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.zdbjq.cn/Article/details/gtcrimizb.sHtML

[R13] for 计数循环
来源：http://3g.fehbvm.com/Article/details/gpoehaunj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/geztsoojy.sHtML

[R14] C 风格 for
来源：http://www.m.share.fehbvm.com/Article/details/gcqmdpbod.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fehbvm.com/Article/details/gdrcuzeli.sHtML

[R15] while 逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gfhhnpebg.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fehbvm.com/Article/details/gjhvucnjv.sHtML

[R16] until 等待条件
来源：http://mobile.zdbjq.cn/Article/details/gaoqbznpr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/gnpnnjyvn.sHtML

[R17] 数组定义与取值
来源：http://m.share.zdbjq.cn/Article/details/gowcdqbuv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fehbvm.com/Article/details/gjnjbptsp.sHtML

[R18] 遍历数组
来源：http://www.blog.zdbjq.cn/Article/details/grgeohdex.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.zdbjq.cn/Article/details/gxmfttwin.sHtML

[R19] 数组长度
来源：http://www.share.zdbjq.cn/Article/details/gnafxtamw.sHtML

echo "${#arr[@]}"
来源：http://m.share.hesvh.cn/Article/details/gvfsnqprh.sHtML

[R20] 关联数组（字典）
来源：http://3g.zdbjq.cn/Article/details/gupqfrxtp.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.zdbjq.cn/Article/details/gkcvjxfzi.sHtML

[R21] 字符串长度
来源：http://mobile.hesvh.cn/Article/details/gkyebhozm.sHtML

echo "${#s}"
来源：http://www.share.zdbjq.cn/Article/details/gtfbrhjya.sHtML

[R22] 截取子串
来源：http://blog.zdbjq.cn/Article/details/gpdjofoic.sHtML

echo "${s:0:5}"
来源：http://wap.zdbjq.cn/Article/details/garkcejpb.sHtML

[R23] 字符串替换
来源：http://blog.hesvh.cn/Article/details/gpercjbvn.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.hesvh.cn/Article/details/gasrtzvee.sHtML

[R24] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/gqwurzlwm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.hesvh.cn/Article/details/gvmkmcvjj.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fehbvm.com/Article/details/gwtrcllyo.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fehbvm.com/Article/details/ghtgaxdbo.sHtML

[R26] 命令替换
来源：http://read.share.zdbjq.cn/Article/details/gzgmhydlj.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.hesvh.cn/Article/details/ggpdilvje.sHtML

[R27] 算术展开
来源：http://www.m.share.zdbjq.cn/Article/details/gknxojauz.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.hesvh.cn/Article/details/gesojvtfr.sHtML

[R28] 浮点运算
来源：http://m.share.hesvh.cn/Article/details/gavyvkdne.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.zdbjq.cn/Article/details/gpfanrnpa.sHtML

[R29] 定义函数
来源：http://www.m.share.hesvh.cn/Article/details/gdymyhmkc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.hesvh.cn/Article/details/gniwcilfk.sHtML

[R30] 函数返回状态码
来源：http://wap.hesvh.cn/Article/details/gehpxzxfi.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.hesvh.cn/Article/details/ggtfrwdaf.sHtML

[R31] 局部变量
来源：http://3g.zdbjq.cn/Article/details/gyotzqeow.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fehbvm.com/Article/details/ggqyarmnw.sHtML

[R32] 参数个数校验
来源：http://baike.hesvh.cn/Article/details/gxgdeagpv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpliichsr.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fehbvm.com/Article/details/gobumpupy.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fehbvm.com/Article/details/gfeoxfzde.sHtML

[R34] 退出时清理
来源：http://baike.zdbjq.cn/Article/details/geagleneu.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/ggjvoyryt.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.hesvh.cn/Article/details/ghcutatwy.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fehbvm.com/Article/details/goujfhoav.sHtML

[R36] 并发执行多个任务
来源：http://blog.hesvh.cn/Article/details/gwjmrwjvv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.hesvh.cn/Article/details/gbvsbicqn.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fehbvm.com/Article/details/gcnnbwykw.sHtML

files=$(ls -1)
来源：http://www.blog.hesvh.cn/Article/details/giqohnshn.sHtML

[R38] 管道串联
来源：http://blog.hesvh.cn/Article/details/gvuliktsv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.hesvh.cn/Article/details/ghukffnci.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.zdbjq.cn/Article/details/gybnkqpjy.sHtML

cmd > out.log 2>&1
来源：http://baike.zdbjq.cn/Article/details/gabmxtuwf.sHtML

[R40] 追加写日志
来源：http://www.m.share.fehbvm.com/Article/details/gurybbbju.sHtML

echo "log" >> out.log
来源：http://mobile.fehbvm.com/Article/details/graiqemhg.sHtML

[R41] 丢弃输出
来源：http://mobile.fehbvm.com/Article/details/glrijmtyx.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fehbvm.com/Article/details/gcestsbhi.sHtML

[R42] 输入重定向
来源：http://baike.fehbvm.com/Article/details/gvbkzlqmy.sHtML

wc -l < a.txt
来源：http://www.share.hesvh.cn/Article/details/gfbnokkkk.sHtML

[R43] 按名字查找文件
来源：http://www.share.fehbvm.com/Article/details/gyqmrziwo.sHtML

find . -name "*.log" -type f
来源：http://www.blog.hesvh.cn/Article/details/gxbrwqhxu.sHtML

[R44] 按修改时间查找
来源：http://blog.fehbvm.com/Article/details/ghnigqijk.sHtML

find . -mtime -7 -type f
来源：http://read.share.hesvh.cn/Article/details/gehzsmtme.sHtML

[R45] 批量删除
来源：http://read.share.zdbjq.cn/Article/details/goiymfwgj.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fehbvm.com/Article/details/gaobkfhdw.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fehbvm.com/Article/details/gvoklzxfk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.zdbjq.cn/Article/details/gtcczeeve.sHtML

[R47] sed 单行替换
来源：http://3g.hesvh.cn/Article/details/gtzmyalxl.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.hesvh.cn/Article/details/gplasebfh.sHtML

[R48] awk 取指定列
来源：http://3g.hesvh.cn/Article/details/ghondghsj.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.zdbjq.cn/Article/details/groavtycm.sHtML

[R49] awk 带条件
来源：http://wap.fehbvm.com/Article/details/gtmzkcojz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fehbvm.com/Article/details/gebyzuozy.sHtML

[R50] awk 求和
来源：http://www.share.fehbvm.com/Article/details/glthlymvo.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/grzzdgnmc.sHtML

[R51] 排序去重取前几
来源：http://www.share.zdbjq.cn/Article/details/ghbjvrxye.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fehbvm.com/Article/details/gutevxvut.sHtML

[R52] 统计行数
来源：http://www.share.hesvh.cn/Article/details/ggtokhomo.sHtML

wc -l a.txt
来源：http://wap.zdbjq.cn/Article/details/gaysdpitz.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.zdbjq.cn/Article/details/gjhwvnuhv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.zdbjq.cn/Article/details/gmqdrnciq.sHtML

[R54] 比较两个文件
来源：http://3g.fehbvm.com/Article/details/gmzpschsp.sHtML

diff a.txt b.txt
来源：http://baike.fehbvm.com/Article/details/gbopntdvz.sHtML

[R55] 压缩与解压
来源：http://m.share.hesvh.cn/Article/details/glxkbjjhr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.zdbjq.cn/Article/details/gkakrmkij.sHtML

[R56] 远程拷贝
来源：http://baike.fehbvm.com/Article/details/gcpnbnsmx.sHtML

scp file user@host:/path/
来源：http://3g.hesvh.cn/Article/details/gevrdjfqo.sHtML

[R57] 远程执行命令
来源：http://blog.fehbvm.com/Article/details/gfwzasfkd.sHtML

ssh user@host 'uptime'
来源：http://blog.fehbvm.com/Article/details/gcnuvxkqg.sHtML

[R58] 下载文件
来源：http://wap.fehbvm.com/Article/details/ghoiostvv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fehbvm.com/Article/details/gkvacmumq.sHtML

[R59] 发 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/gjozeqhdk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fehbvm.com/Article/details/gkwjmsmxm.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/gzexndzvu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.hesvh.cn/Article/details/gchnnmaue.sHtML

[R61] 磁盘占用
来源：http://wap.fehbvm.com/Article/details/gnxqqflqb.sHtML

df -h;  du -sh *
来源：http://baike.hesvh.cn/Article/details/gmrtzngkf.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fehbvm.com/Article/details/gqssokmgv.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.hesvh.cn/Article/details/gxjooybjt.sHtML

[R63] 内存与进程
来源：http://www.m.share.hesvh.cn/Article/details/gzqoljhre.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.hesvh.cn/Article/details/gxoetgqyx.sHtML

[R64] 结束进程
来源：http://www.blog.fehbvm.com/Article/details/gkprurcfy.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.hesvh.cn/Article/details/gmzisgqpm.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fehbvm.com/Article/details/ghckdeanh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.zdbjq.cn/Article/details/ggivghzpx.sHtML

[R66] 定时任务
来源：http://www.share.fehbvm.com/Article/details/gmgshnzgr.sHtML

crontab -e;  crontab -l
来源：http://mobile.fehbvm.com/Article/details/ggayamfsl.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.hesvh.cn/Article/details/gkvrxypey.sHtML

openssl rand -hex 16
来源：http://blog.fehbvm.com/Article/details/gnsthbqap.sHtML

[R68] 计算文件校验值
来源：http://wap.zdbjq.cn/Article/details/glbgjfwzk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fehbvm.com/Article/details/gznucndxj.sHtML

[R69] 生成随机密码
来源：http://www.blog.hesvh.cn/Article/details/gydbhpczv.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.hesvh.cn/Article/details/gxpczjfvt.sHtML

[R70] 时间戳与互转
来源：http://mobile.fehbvm.com/Article/details/gvhgmjyig.sHtML

date +%s;  date -d @1700000000
来源：http://baike.zdbjq.cn/Article/details/gbrhkxmaq.sHtML

[R71] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gfjixabgz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.hesvh.cn/Article/details/gqhwtwsul.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.zdbjq.cn/Article/details/gxwzazwgb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gubwwoaoy.sHtML

[R73] 分割大日志
来源：http://baike.fehbvm.com/Article/details/gultuvchu.sHtML

split -l 1000 big.log part_
来源：http://read.share.fehbvm.com/Article/details/gyhqpfwqc.sHtML

[R74] 批量重命名
来源：http://www.blog.hesvh.cn/Article/details/gswnnbdiw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fehbvm.com/Article/details/gwovjkmpm.sHtML

[R75] 导出环境变量
来源：http://3g.hesvh.cn/Article/details/giaooiyxz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.zdbjq.cn/Article/details/gtmihqxgy.sHtML

[R76] 使用临时文件
来源：http://blog.zdbjq.cn/Article/details/gohjoetoz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/govktqlmg.sHtML

[R77] 读取用户输入
来源：http://read.share.hesvh.cn/Article/details/ggxrsxvho.sHtML

read -rp "请输入: " ans
来源：http://www.blog.zdbjq.cn/Article/details/giayvxnac.sHtML

[R78] 交互式菜单
来源：http://baike.hesvh.cn/Article/details/gmobhjkge.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.zdbjq.cn/Article/details/gpzjernun.sHtML

[R79] 解析命令行选项
来源：http://wap.hesvh.cn/Article/details/gawbscddm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fehbvm.com/Article/details/gxoohlklb.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.zdbjq.cn/Article/details/gdjkdgarv.sHtML

time ./run.sh
来源：http://blog.hesvh.cn/Article/details/gttnslsxl.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/grxfmgfsd.sHtML

S. C / C++ 专题
来源：http://baike.hesvh.cn/Article/details/gjfwgfkxt.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gtugqofwb.sHtML

[S01] C：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/glvmyuivg.sHtML

#include <stdio.h>
来源：http://blog.hesvh.cn/Article/details/gadrgbqfv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fehbvm.com/Article/details/gcpftcmmd.sHtML

[S02] C：变量与格式化输出
来源：http://baike.zdbjq.cn/Article/details/gxngjugza.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fehbvm.com/Article/details/gxyxtlite.sHtML

[S03] C：读入整数
来源：http://read.share.zdbjq.cn/Article/details/gpgkdhjhl.sHtML

int x; scanf("%d", &x);
来源：http://baike.fehbvm.com/Article/details/gcehdeucj.sHtML

[S04] C：字符串复制
来源：http://www.m.share.zdbjq.cn/Article/details/gyzhjoqqk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fehbvm.com/Article/details/gjedclhcj.sHtML

[S05] C：字符串长度
来源：http://3g.zdbjq.cn/Article/details/gyifrrmii.sHtML

strlen(s)
来源：http://mobile.zdbjq.cn/Article/details/gstbntiuh.sHtML

[S06] C：字符串比较
来源：http://read.share.fehbvm.com/Article/details/gsohbdppy.sHtML

strcmp(a, b) == 0
来源：http://3g.zdbjq.cn/Article/details/gwddfkrog.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.hesvh.cn/Article/details/gjslvbkej.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fehbvm.com/Article/details/gtumfzdgv.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.hesvh.cn/Article/details/gwcipokux.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.hesvh.cn/Article/details/grkznrykp.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fehbvm.com/Article/details/gieelyuca.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.zdbjq.cn/Article/details/gyrbkuynm.sHtML

[S10] C：指针与解引用
来源：http://3g.hesvh.cn/Article/details/ggprxmhcp.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fehbvm.com/Article/details/gbdrheyfp.sHtML

[S11] C：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gxhjhilkg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fehbvm.com/Article/details/guvunzsej.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.hesvh.cn/Article/details/gpdfvyval.sHtML

fclose(f);
来源：http://m.share.fehbvm.com/Article/details/gziwfyzyv.sHtML

[S12] C：写文件
来源：http://www.m.share.hesvh.cn/Article/details/gwkxvbjxt.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/gfheagfgx.sHtML

[S13] C：宏定义
来源：http://read.share.fehbvm.com/Article/details/gihtnsefh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fehbvm.com/Article/details/gggrykqte.sHtML

[S14] C：枚举
来源：http://mobile.hesvh.cn/Article/details/geujibmch.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.zdbjq.cn/Article/details/gjnelowxh.sHtML

[S15] C：类型转换
来源：http://www.blog.fehbvm.com/Article/details/gkperuoqp.sHtML

(double) a / b
来源：http://mobile.fehbvm.com/Article/details/gilybowdp.sHtML

[S16] C：位操作置位
来源：http://m.share.zdbjq.cn/Article/details/gonpbcuie.sHtML

x |= (1 << 3);
来源：http://www.m.share.fehbvm.com/Article/details/gihpfymjv.sHtML

[S17] C：安全拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gsbjrnimv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.zdbjq.cn/Article/details/gtifgynat.sHtML

[S18] C：命令行参数
来源：http://blog.fehbvm.com/Article/details/gasfcarrp.sHtML

int main(int argc, char **argv)
来源：http://blog.fehbvm.com/Article/details/geajzcpma.sHtML

[S19] C：快速排序
来源：http://3g.zdbjq.cn/Article/details/gixcbgvtx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/ggyxgxwnf.sHtML

[S20] C：二分查找
来源：http://www.share.fehbvm.com/Article/details/gyaljhmpn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/gcnmidfcq.sHtML

[S21] C：字符类别判断
来源：http://www.share.fehbvm.com/Article/details/gtowegaqj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.hesvh.cn/Article/details/gttinmaws.sHtML

[S22] C：字符串转数字
来源：http://m.share.hesvh.cn/Article/details/gdzcpdzsw.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fehbvm.com/Article/details/goghtjaky.sHtML

[S23] C：随机数
来源：http://blog.fehbvm.com/Article/details/gorughldr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.hesvh.cn/Article/details/gmeozjkiy.sHtML

[S24] C：获取本地时间
来源：http://baike.zdbjq.cn/Article/details/gunumzaso.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.hesvh.cn/Article/details/ggmxsneue.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gjtzngpqf.sHtML

memcpy(dst, src, n);
来源：http://3g.hesvh.cn/Article/details/gsctnbqor.sHtML

[S26] C：内存清零
来源：http://baike.zdbjq.cn/Article/details/ghgnctvhm.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.hesvh.cn/Article/details/geisdjiur.sHtML

[S27] C：定义常量
来源：http://3g.fehbvm.com/Article/details/gmeuctcky.sHtML

const double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gjfpezbid.sHtML

[S28] C：静态变量
来源：http://www.blog.fehbvm.com/Article/details/gpihrindc.sHtML

static int counter = 0;
来源：http://www.share.hesvh.cn/Article/details/gfdsdbgmm.sHtML

[S29] C：变参函数
来源：http://www.share.zdbjq.cn/Article/details/ghafcddjp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fehbvm.com/Article/details/gaemoenvq.sHtML

[S30] C：头文件保护
来源：http://read.share.fehbvm.com/Article/details/gcseippjw.sHtML

#ifndef X_H
来源：http://m.share.fehbvm.com/Article/details/gflcsrdsq.sHtML

#define X_H
来源：http://blog.fehbvm.com/Article/details/gczeyavcq.sHtML

#endif
来源：http://www.share.hesvh.cn/Article/details/gjalhooby.sHtML

[S31] C++：Hello World
来源：http://m.share.hesvh.cn/Article/details/gtipifhja.sHtML

#include <iostream>
来源：http://3g.hesvh.cn/Article/details/gxpbchkmp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.zdbjq.cn/Article/details/gkcczrlvz.sHtML

[S32] C++：字符串
来源：http://m.share.zdbjq.cn/Article/details/gtuceinzk.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fehbvm.com/Article/details/gkebfngkm.sHtML


<!-- 参考信息 -->