代发 wailian999

[Q65] 回滚事务
来源：http://wap.fanxiaobao.xyz/Article/details/gvrtuocxn.sHtML

ROLLBACK;
来源：http://wap.fanxiaobao.xyz/Article/details/gzksvclbl.sHtML

[Q66] 行锁查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqnhcazbw.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fanxiaobao.xyz/Article/details/gaqjzntiv.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fanxiaobao.xyz/Article/details/gqwajnppz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fanxiaobao.xyz/Article/details/gavvnuujw.sHtML

[Q68] 保存点
来源：http://mobile.fanxiaobao.xyz/Article/details/gumsemfpl.sHtML

SAVEPOINT sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsrgmvqly.sHtML

ROLLBACK TO sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/ghysljzlc.sHtML

[Q69] 查看执行计划
来源：http://mobile.fanxiaobao.xyz/Article/details/gkvorupxz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fanxiaobao.xyz/Article/details/geukkszcq.sHtML

[Q70] 更新统计信息
来源：http://read.share.fanxiaobao.xyz/Article/details/gterfdzfn.sHtML

ANALYZE TABLE users;
来源：http://3g.fanxiaobao.xyz/Article/details/gnhuzwswh.sHtML

[Q71] 查看建表语句
来源：http://blog.fanxiaobao.xyz/Article/details/gomtyjndp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gftaaaads.sHtML

[Q72] 查看索引
来源：http://read.share.fanxiaobao.xyz/Article/details/ghumehlpr.sHtML

SHOW INDEX FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gohdvvnbl.sHtML

[Q73] 查看表状态
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdkghbanw.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gplrahfur.sHtML

[Q74] 强制使用索引
来源：http://3g.fanxiaobao.xyz/Article/details/gtdbwtnmd.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fanxiaobao.xyz/Article/details/gvtcbcdzf.sHtML

[Q75] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gxnfbvjpg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/geallbabd.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyqctpdzu.sHtML

[Q76] 按天统计
来源：http://wap.fanxiaobao.xyz/Article/details/ghaejdpgj.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fanxiaobao.xyz/Article/details/gyeyklagb.sHtML

[Q77] 时间加减
来源：http://baike.fanxiaobao.xyz/Article/details/gsddiggff.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fanxiaobao.xyz/Article/details/gavfrtpnf.sHtML

[Q78] 当前时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gpqqlmoym.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqyyvbib.sHtML

[Q79] 字符串拼接
来源：http://m.share.fanxiaobao.xyz/Article/details/gdzhujzec.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fanxiaobao.xyz/Article/details/gcqqjujjq.sHtML

[Q80] 字符串截取
来源：http://www.share.fanxiaobao.xyz/Article/details/gffpvztwb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gdkqttzzf.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqphwddtm.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzdvkutoq.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fanxiaobao.xyz/Article/details/gwzwzxltq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtmhkpckt.sHtML

[Q83] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gfvdqamop.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhjtxydy.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fanxiaobao.xyz/Article/details/gztsbvzxp.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gslrdzieg.sHtML

[Q85] 数值取整
来源：http://read.share.fanxiaobao.xyz/Article/details/guckqgoaf.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbshdkfun.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxewkqxgy.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fanxiaobao.xyz/Article/details/guypobsoa.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghnfentta.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fanxiaobao.xyz/Article/details/gxevfkmos.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.fanxiaobao.xyz/Article/details/gruudkkdg.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fanxiaobao.xyz/Article/details/gmazvriir.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gczfexszc.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gjgnsjzis.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyoammuqe.sHtML

[Q90] 生成序号列
来源：http://3g.fanxiaobao.xyz/Article/details/gycfviyud.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggfylxthu.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gysxqlzbg.sHtML

R. Bash 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gglabauki.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqajreter.sHtML

[R01] shebang 与严格模式
来源：http://3g.fanxiaobao.xyz/Article/details/gcinmdhbu.sHtML

#!/usr/bin/env bash
来源：http://m.share.fanxiaobao.xyz/Article/details/gzoygynhf.sHtML

set -euo pipefail
来源：http://3g.fanxiaobao.xyz/Article/details/gtiopapmt.sHtML

[R02] 变量赋值与使用
来源：http://blog.fanxiaobao.xyz/Article/details/gmzvzpbgb.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/guyvioloq.sHtML

[R03] 只读变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gasoocxam.sHtML

readonly PI=3.14
来源：http://mobile.fanxiaobao.xyz/Article/details/gxladosyd.sHtML

[R04] 位置参数
来源：http://read.share.fanxiaobao.xyz/Article/details/goruwdejf.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fanxiaobao.xyz/Article/details/gnnrpcbcj.sHtML

[R05] 参数默认值
来源：http://3g.fanxiaobao.xyz/Article/details/gatkmubpo.sHtML

name="${1:-default}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyqivxagj.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gnzyxfogn.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/ggvcxognc.sHtML

[R07] if 判断文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gmeevlwpy.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbrszyys.sHtML

[R08] 数值比较
来源：http://wap.fanxiaobao.xyz/Article/details/gyybqedzn.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnoevcfxd.sHtML

[R09] 字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gnoupktbv.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gfzqxbzda.sHtML

[R10] 正则匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gyakebevz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqotexbdu.sHtML

[R11] case 多分支
来源：http://m.share.fanxiaobao.xyz/Article/details/goqblcqck.sHtML

case "$1" in
来源：http://read.share.fanxiaobao.xyz/Article/details/guypsdgsd.sHtML

start) echo "启动" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvedphqvu.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gznnrlhxo.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqqpjwenp.sHtML

esac
来源：http://3g.fanxiaobao.xyz/Article/details/gifyehfoo.sHtML

[R12] for 遍历文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gshlkijvi.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gruelzgva.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gswxybajt.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gvqucqwgu.sHtML

[R14] C 风格 for
来源：http://read.share.fanxiaobao.xyz/Article/details/gzidtppzs.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gxgdnaidl.sHtML

[R15] while 逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gpmipjavg.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gsaavelwd.sHtML

[R16] until 等待条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gncbghziz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gokiipngi.sHtML

[R17] 数组定义与取值
来源：http://baike.fanxiaobao.xyz/Article/details/gbyzyexqq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gytyygeij.sHtML

[R18] 遍历数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gqgxfqpcp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmlxheapz.sHtML

[R19] 数组长度
来源：http://3g.fanxiaobao.xyz/Article/details/gzdyndsvl.sHtML

echo "${#arr[@]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gskvxyqdb.sHtML

[R20] 关联数组（字典）
来源：http://3g.fanxiaobao.xyz/Article/details/ghruytkxj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsrvgrhgy.sHtML

[R21] 字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gahnyjakm.sHtML

echo "${#s}"
来源：http://wap.fanxiaobao.xyz/Article/details/gajrkncmt.sHtML

[R22] 截取子串
来源：http://wap.fanxiaobao.xyz/Article/details/gyexgmhrn.sHtML

echo "${s:0:5}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtjuzdbb.sHtML

[R23] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gqmqfsrmq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gzeiqabsr.sHtML

[R24] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gayhuzibi.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fanxiaobao.xyz/Article/details/guepbukpz.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/gwyqqfpth.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gjogmqhhh.sHtML

[R26] 命令替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/garilqveb.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fanxiaobao.xyz/Article/details/gbwsejcsx.sHtML

[R27] 算术展开
来源：http://3g.fanxiaobao.xyz/Article/details/gquzblmbh.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfetsvyf.sHtML

[R28] 浮点运算
来源：http://blog.fanxiaobao.xyz/Article/details/gcfiwpzkd.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fanxiaobao.xyz/Article/details/geyadruyy.sHtML

[R29] 定义函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbrahyaa.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gidihhjsm.sHtML

[R30] 函数返回状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gobanyuxr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtalpohiv.sHtML

[R31] 局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gfqgpejdu.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gapbpkmhd.sHtML

[R32] 参数个数校验
来源：http://mobile.fanxiaobao.xyz/Article/details/gnuueuvul.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggstiupmb.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fanxiaobao.xyz/Article/details/gfhgjvpbb.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fanxiaobao.xyz/Article/details/gypaxhxju.sHtML

[R34] 退出时清理
来源：http://3g.fanxiaobao.xyz/Article/details/grawwqbln.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggdmhdvam.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaiazoqce.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fanxiaobao.xyz/Article/details/ghnzhxyqz.sHtML

[R36] 并发执行多个任务
来源：http://blog.fanxiaobao.xyz/Article/details/govsxvbjn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fanxiaobao.xyz/Article/details/gyytfvpsp.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqybxssek.sHtML

files=$(ls -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmixhpokb.sHtML

[R38] 管道串联
来源：http://www.share.fanxiaobao.xyz/Article/details/gfncoqngz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fanxiaobao.xyz/Article/details/glegqomqq.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fanxiaobao.xyz/Article/details/glkdqbqoe.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gtdobjoad.sHtML

[R40] 追加写日志
来源：http://3g.fanxiaobao.xyz/Article/details/gpdfbrldr.sHtML

echo "log" >> out.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gfupadjst.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/giubjjidy.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gifwthokd.sHtML

[R42] 输入重定向
来源：http://www.share.fanxiaobao.xyz/Article/details/gqdsmrxdj.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfdzyskle.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmxqncyzv.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giisbmvkx.sHtML

[R44] 按修改时间查找
来源：http://www.share.fanxiaobao.xyz/Article/details/ghahlxjtv.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gnffoeiff.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/gbnohsxke.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fanxiaobao.xyz/Article/details/gjnjwgrgc.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fanxiaobao.xyz/Article/details/giesqwxep.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/greuuhwrj.sHtML

[R47] sed 单行替换
来源：http://baike.fanxiaobao.xyz/Article/details/gcoweqjjm.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/glgsuobga.sHtML

[R48] awk 取指定列
来源：http://blog.fanxiaobao.xyz/Article/details/gcudtivba.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/grlpwuwfp.sHtML

[R49] awk 带条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmdowrpqn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fanxiaobao.xyz/Article/details/givolsxux.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxpztcirr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzpiyqxyy.sHtML

[R51] 排序去重取前几
来源：http://baike.fanxiaobao.xyz/Article/details/gfyuacacy.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fanxiaobao.xyz/Article/details/gyhwlqzas.sHtML

[R52] 统计行数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnyehjspf.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gcykfknyp.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmseniydq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gqzbvgisq.sHtML

[R54] 比较两个文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gxcsjipan.sHtML

diff a.txt b.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gdrbspjar.sHtML

[R55] 压缩与解压
来源：http://baike.fanxiaobao.xyz/Article/details/gvhmozfao.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fanxiaobao.xyz/Article/details/gbpgvlqvp.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtcshkhye.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/gsltmttny.sHtML

[R57] 远程执行命令
来源：http://wap.fanxiaobao.xyz/Article/details/gbbcjvuwi.sHtML

ssh user@host 'uptime'
来源：http://blog.fanxiaobao.xyz/Article/details/gemhdemhb.sHtML

[R58] 下载文件
来源：http://baike.fanxiaobao.xyz/Article/details/garsgzjpx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fanxiaobao.xyz/Article/details/glixdxnqg.sHtML

[R59] 发 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gdaubyzrb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fanxiaobao.xyz/Article/details/gnvfbhlig.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gkobfywsq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gaujxiobn.sHtML

[R61] 磁盘占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gtgayeocb.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/gudfcomxe.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gyygwnxld.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzlqaqkcj.sHtML

[R63] 内存与进程
来源：http://blog.fanxiaobao.xyz/Article/details/gwbsulzyt.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fanxiaobao.xyz/Article/details/gbpoxeqnh.sHtML

[R64] 结束进程
来源：http://3g.fanxiaobao.xyz/Article/details/ghzjcogql.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqlnhaiwu.sHtML

[R65] 查看端口占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmbwolql.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/gwrjktrdz.sHtML

[R66] 定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqkequcog.sHtML

crontab -e;  crontab -l
来源：http://wap.fanxiaobao.xyz/Article/details/goiiwwacq.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fanxiaobao.xyz/Article/details/gpelnobfz.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/gzxgiwdfx.sHtML

[R68] 计算文件校验值
来源：http://blog.fanxiaobao.xyz/Article/details/gioqtdkpq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gwwtxkkfg.sHtML

[R69] 生成随机密码
来源：http://www.share.fanxiaobao.xyz/Article/details/ggsekhxmz.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fanxiaobao.xyz/Article/details/gshfrhufr.sHtML

[R70] 时间戳与互转
来源：http://read.share.fanxiaobao.xyz/Article/details/gaybcimqx.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fanxiaobao.xyz/Article/details/gmbwmhbax.sHtML

[R71] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gjktdmacv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fanxiaobao.xyz/Article/details/gysmwysix.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/gkiqwhtgm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvglmqlj.sHtML

[R73] 分割大日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywqfwqjb.sHtML

split -l 1000 big.log part_
来源：http://3g.fanxiaobao.xyz/Article/details/gudqepirr.sHtML

[R74] 批量重命名
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzapekuje.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gtgqlhrsg.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gqvzccuim.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/gddvpbemz.sHtML

[R76] 使用临时文件
来源：http://wap.fanxiaobao.xyz/Article/details/gjshcxlgh.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/girovtrhm.sHtML

[R77] 读取用户输入
来源：http://mobile.fanxiaobao.xyz/Article/details/gbgrlubjw.sHtML

read -rp "请输入: " ans
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmrztpun.sHtML

[R78] 交互式菜单
来源：http://baike.fanxiaobao.xyz/Article/details/gadzozeac.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gpqhiwirs.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/gicwzqjmy.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fanxiaobao.xyz/Article/details/ghjhfupna.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvbzncqo.sHtML

time ./run.sh
来源：http://baike.fanxiaobao.xyz/Article/details/glginvdfn.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gowshvcoa.sHtML

S. C / C++ 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gcnzjibdr.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/glfdmqkuk.sHtML

[S01] C：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvcwmnam.sHtML

#include <stdio.h>
来源：http://wap.fanxiaobao.xyz/Article/details/ghyifavcv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fanxiaobao.xyz/Article/details/grolwbjgn.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gmrvnawin.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fanxiaobao.xyz/Article/details/glofnygoz.sHtML

[S03] C：读入整数
来源：http://baike.fanxiaobao.xyz/Article/details/gjhtgrueu.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwrurwecb.sHtML

[S04] C：字符串复制
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzxhhpkk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/ghafanqei.sHtML

[S05] C：字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gursmgmzu.sHtML

strlen(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gwcvndmse.sHtML

[S06] C：字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gdwfofyxt.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/gucenfyki.sHtML

[S07] C：数组遍历求和
来源：http://blog.fanxiaobao.xyz/Article/details/gusqxviaz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/gsatcroow.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fanxiaobao.xyz/Article/details/gccsjogxk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fanxiaobao.xyz/Article/details/gfjucmmvd.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fanxiaobao.xyz/Article/details/gukumwdcr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fanxiaobao.xyz/Article/details/gxehrieuk.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fanxiaobao.xyz/Article/details/geylziuey.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdwvaimls.sHtML

[S11] C：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gabmikxwk.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxaakzwke.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbtsicduz.sHtML

fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gfoysttuz.sHtML

[S12] C：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjwxnues.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghnpbcdvf.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gsoytwfbm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fanxiaobao.xyz/Article/details/ghyastdot.sHtML

[S14] C：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gwaytjkmb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fanxiaobao.xyz/Article/details/gxhexnhsn.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gteakmlge.sHtML

(double) a / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grrtctyxv.sHtML

[S16] C：位操作置位
来源：http://blog.fanxiaobao.xyz/Article/details/gpbmfbwjd.sHtML

x |= (1 << 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjbguvcf.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbxwlnmle.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fanxiaobao.xyz/Article/details/gmvnvjxsm.sHtML

[S18] C：命令行参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gopyfmcgp.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gktwgeaxg.sHtML

[S19] C：快速排序
来源：http://3g.fanxiaobao.xyz/Article/details/gdbppheze.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvtxngzt.sHtML

[S20] C：二分查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gfhzalrzc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gznjeghfi.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gknqyrqdm.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/glryxwatb.sHtML

[S22] C：字符串转数字
来源：http://3g.fanxiaobao.xyz/Article/details/gjdvwvvhc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fanxiaobao.xyz/Article/details/grmgidokl.sHtML

[S23] C：随机数
来源：http://wap.fanxiaobao.xyz/Article/details/gyjyoyske.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfejtqfgk.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxcdtsjw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fanxiaobao.xyz/Article/details/gvyetdura.sHtML

[S25] C：内存拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gilceioop.sHtML

memcpy(dst, src, n);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqynltypo.sHtML

[S26] C：内存清零
来源：http://blog.fanxiaobao.xyz/Article/details/galicxage.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fanxiaobao.xyz/Article/details/gmvwgpcvx.sHtML

[S27] C：定义常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gqigpaffw.sHtML

const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gccaupazv.sHtML

[S28] C：静态变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gkoiwnyaa.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwotuser.sHtML

[S29] C：变参函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxcoordy.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/gyagfkjec.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghhnzamva.sHtML

#ifndef X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjrjqtgf.sHtML

#define X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gutvihnlo.sHtML

#endif
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gigfnkktu.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/ghzvqpbxs.sHtML

#include <iostream>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwpnorpsf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gcqxxvcmm.sHtML

[S32] C++：字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbgrxvnl.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fanxiaobao.xyz/Article/details/gcdqmhpyh.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghmqzvxho.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fanxiaobao.xyz/Article/details/ghhtckmvw.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwunbtfc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fanxiaobao.xyz/Article/details/grjqtijdo.sHtML


<!-- 参考信息 -->