代发 wailian999

[Q63] 开启事务
来源：http://read.share.zdbjq.cn/Article/details/gpmdbbeoy.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.zdbjq.cn/Article/details/gmvccdkim.sHtML

[Q64] 提交事务
来源：http://read.share.hesvh.cn/Article/details/gyttclbfm.sHtML

COMMIT;
来源：http://3g.hesvh.cn/Article/details/gtpeweeot.sHtML

[Q65] 回滚事务
来源：http://mobile.fehbvm.com/Article/details/gkpqjjtye.sHtML

ROLLBACK;
来源：http://read.share.hesvh.cn/Article/details/gyqbaezlu.sHtML

[Q66] 行锁查询
来源：http://baike.fehbvm.com/Article/details/gvizeimon.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.hesvh.cn/Article/details/gfkzeqzwv.sHtML

[Q67] 设置隔离级别
来源：http://3g.fehbvm.com/Article/details/gzyuyttmh.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.hesvh.cn/Article/details/gjkadlngh.sHtML

[Q68] 保存点
来源：http://m.share.hesvh.cn/Article/details/giitpvmeu.sHtML

SAVEPOINT sp1;
来源：http://m.share.fehbvm.com/Article/details/gtbttaekq.sHtML

ROLLBACK TO sp1;
来源：http://3g.zdbjq.cn/Article/details/gpbnttsya.sHtML

[Q69] 查看执行计划
来源：http://blog.hesvh.cn/Article/details/gipihlsmx.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.zdbjq.cn/Article/details/gpdawfeuo.sHtML

[Q70] 更新统计信息
来源：http://blog.fehbvm.com/Article/details/gpybfcsqr.sHtML

ANALYZE TABLE users;
来源：http://3g.fehbvm.com/Article/details/gpnzjrtql.sHtML

[Q71] 查看建表语句
来源：http://blog.fehbvm.com/Article/details/gcryqevby.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.zdbjq.cn/Article/details/gtchnukdn.sHtML

[Q72] 查看索引
来源：http://wap.hesvh.cn/Article/details/gqbmierow.sHtML

SHOW INDEX FROM users;
来源：http://3g.hesvh.cn/Article/details/gyemkmrny.sHtML

[Q73] 查看表状态
来源：http://read.share.zdbjq.cn/Article/details/gwyxymshw.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.hesvh.cn/Article/details/gqvixsahy.sHtML

[Q74] 强制使用索引
来源：http://baike.hesvh.cn/Article/details/gitauqlal.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.zdbjq.cn/Article/details/glmuvzona.sHtML

[Q75] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gjfjxqlru.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gyyznwdzy.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.zdbjq.cn/Article/details/gntzrahev.sHtML

[Q76] 按天统计
来源：http://mobile.fehbvm.com/Article/details/gvoozuyoc.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.zdbjq.cn/Article/details/gpldjkksc.sHtML

[Q77] 时间加减
来源：http://m.share.fehbvm.com/Article/details/gulazpfcc.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fehbvm.com/Article/details/ggqssccpk.sHtML

[Q78] 当前时间
来源：http://wap.fehbvm.com/Article/details/gequlehsk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fehbvm.com/Article/details/gmzerrivf.sHtML

[Q79] 字符串拼接
来源：http://baike.fehbvm.com/Article/details/gnkbjbudk.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.zdbjq.cn/Article/details/gzadhgugf.sHtML

[Q80] 字符串截取
来源：http://wap.zdbjq.cn/Article/details/gpaxuobsc.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gurnslbpc.sHtML

[Q81] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gfxnbedtq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.hesvh.cn/Article/details/gfiaaznpz.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.hesvh.cn/Article/details/gsyojynab.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gezhnatex.sHtML

[Q83] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/gvelrhojc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gpjgwbrkm.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fehbvm.com/Article/details/gwsqpgdtf.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/guuazfgry.sHtML

[Q85] 数值取整
来源：http://www.m.share.hesvh.cn/Article/details/gkavigstz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.hesvh.cn/Article/details/gibjigart.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.hesvh.cn/Article/details/gddbjllad.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.hesvh.cn/Article/details/gulqarbgd.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.zdbjq.cn/Article/details/gdshzcxqf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fehbvm.com/Article/details/grcexfiyh.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.hesvh.cn/Article/details/ggenrcgyn.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fehbvm.com/Article/details/gfxjjwyqm.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gdfsclbsz.sHtML

[Q89] 判断表是否存在
来源：http://read.share.hesvh.cn/Article/details/gusyohvdg.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fehbvm.com/Article/details/ghgvedtet.sHtML

[Q90] 生成序号列
来源：http://wap.zdbjq.cn/Article/details/gokxfuosi.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.zdbjq.cn/Article/details/gvpahpbpk.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gakzyiuup.sHtML

R. Bash 专题
来源：http://www.blog.zdbjq.cn/Article/details/gtogvquhl.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/grfhqyrgp.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.hesvh.cn/Article/details/gwfxirpej.sHtML

#!/usr/bin/env bash
来源：http://blog.zdbjq.cn/Article/details/gcxpweuvn.sHtML

set -euo pipefail
来源：http://baike.fehbvm.com/Article/details/gfoskntgd.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fehbvm.com/Article/details/glnbspfrq.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.hesvh.cn/Article/details/geyouayti.sHtML

[R03] 只读变量
来源：http://3g.hesvh.cn/Article/details/guxnilpss.sHtML

readonly PI=3.14
来源：http://www.share.zdbjq.cn/Article/details/ggoqvdhoc.sHtML

[R04] 位置参数
来源：http://www.blog.fehbvm.com/Article/details/genmplcfa.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fehbvm.com/Article/details/gugiqmcnv.sHtML

[R05] 参数默认值
来源：http://www.blog.zdbjq.cn/Article/details/gxtxmpxad.sHtML

name="${1:-default}"
来源：http://mobile.zdbjq.cn/Article/details/gupfbdklq.sHtML

[R06] 判断命令是否存在
来源：http://baike.zdbjq.cn/Article/details/gishstnpb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/ggldqueac.sHtML

[R07] if 判断文件
来源：http://blog.fehbvm.com/Article/details/gaifcjqiw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.hesvh.cn/Article/details/gyshlhvaw.sHtML

[R08] 数值比较
来源：http://3g.fehbvm.com/Article/details/gkgkxvtpg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.zdbjq.cn/Article/details/gpiesdkgf.sHtML

[R09] 字符串比较
来源：http://www.share.hesvh.cn/Article/details/gkjfljyfh.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.zdbjq.cn/Article/details/glamgresj.sHtML

[R10] 正则匹配
来源：http://blog.hesvh.cn/Article/details/ghpbdjqgp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fehbvm.com/Article/details/gikmcvwsw.sHtML

[R11] case 多分支
来源：http://wap.zdbjq.cn/Article/details/gnbgmjpsz.sHtML

case "$1" in
来源：http://wap.fehbvm.com/Article/details/galhhjhwo.sHtML

start) echo "启动" ;;
来源：http://read.share.hesvh.cn/Article/details/gdgixezhw.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gostgmhxr.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fehbvm.com/Article/details/grtijtncc.sHtML

esac
来源：http://blog.zdbjq.cn/Article/details/gwzsgzbxq.sHtML

[R12] for 遍历文件
来源：http://read.share.fehbvm.com/Article/details/gdsaftiji.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.zdbjq.cn/Article/details/gxxtzpgoc.sHtML

[R13] for 计数循环
来源：http://wap.fehbvm.com/Article/details/gtmpoecom.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/ghduioumk.sHtML

[R14] C 风格 for
来源：http://www.blog.hesvh.cn/Article/details/gijusrkvg.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/gsyeedtgh.sHtML

[R15] while 逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gvefelqdl.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.zdbjq.cn/Article/details/gvbkhsyuw.sHtML

[R16] until 等待条件
来源：http://mobile.hesvh.cn/Article/details/gjyscshan.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/ggkcmavyu.sHtML

[R17] 数组定义与取值
来源：http://mobile.zdbjq.cn/Article/details/gtbwigjxp.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.zdbjq.cn/Article/details/gktgtlyeh.sHtML

[R18] 遍历数组
来源：http://3g.zdbjq.cn/Article/details/gpnhlducd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fehbvm.com/Article/details/gxnstaquf.sHtML

[R19] 数组长度
来源：http://www.m.share.fehbvm.com/Article/details/gomshhsbt.sHtML

echo "${#arr[@]}"
来源：http://m.share.fehbvm.com/Article/details/gwbiywzjl.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fehbvm.com/Article/details/grlpdpuwe.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.zdbjq.cn/Article/details/gqngojtnw.sHtML

[R21] 字符串长度
来源：http://blog.fehbvm.com/Article/details/gqlvqhodw.sHtML

echo "${#s}"
来源：http://www.blog.zdbjq.cn/Article/details/glaqaucsj.sHtML

[R22] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/gxnscynzb.sHtML

echo "${s:0:5}"
来源：http://blog.hesvh.cn/Article/details/gxcncshud.sHtML

[R23] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/gfbcfeuag.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.zdbjq.cn/Article/details/gltpwrtlh.sHtML

[R24] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/ghvozoinl.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fehbvm.com/Article/details/gdkrmswzm.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.hesvh.cn/Article/details/ghbivndli.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fehbvm.com/Article/details/gwyyoggdk.sHtML

[R26] 命令替换
来源：http://www.share.hesvh.cn/Article/details/gzxnrfqrt.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fehbvm.com/Article/details/gucicfpkn.sHtML

[R27] 算术展开
来源：http://www.m.share.fehbvm.com/Article/details/gytgqoddr.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fehbvm.com/Article/details/gvpsbarbq.sHtML

[R28] 浮点运算
来源：http://www.m.share.zdbjq.cn/Article/details/gsoylsfhs.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fehbvm.com/Article/details/gkusryjhh.sHtML

[R29] 定义函数
来源：http://m.share.fehbvm.com/Article/details/gpidfytup.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.hesvh.cn/Article/details/gnhskuvrr.sHtML

[R30] 函数返回状态码
来源：http://3g.fehbvm.com/Article/details/gtgfyuple.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fehbvm.com/Article/details/gtiuomjuj.sHtML

[R31] 局部变量
来源：http://wap.fehbvm.com/Article/details/guoyrxdwz.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.zdbjq.cn/Article/details/grqgtistu.sHtML

[R32] 参数个数校验
来源：http://3g.zdbjq.cn/Article/details/gncwbkcsk.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/gkmvemvdf.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.hesvh.cn/Article/details/giezkjbmm.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.hesvh.cn/Article/details/gcpnljggt.sHtML

[R34] 退出时清理
来源：http://www.share.fehbvm.com/Article/details/gngbchjqj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gsmxkioak.sHtML

[R35] 后台执行并等待
来源：http://baike.fehbvm.com/Article/details/gafpawfws.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.zdbjq.cn/Article/details/gjcbhgbea.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fehbvm.com/Article/details/gucjvvjvo.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.zdbjq.cn/Article/details/gjvvkicrb.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fehbvm.com/Article/details/gzhcycdta.sHtML

files=$(ls -1)
来源：http://www.share.zdbjq.cn/Article/details/ghqstyhov.sHtML

[R38] 管道串联
来源：http://baike.fehbvm.com/Article/details/gcfkcuxml.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.zdbjq.cn/Article/details/grqywhvxu.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.zdbjq.cn/Article/details/gljxodesw.sHtML

cmd > out.log 2>&1
来源：http://www.share.hesvh.cn/Article/details/gemdbvthm.sHtML

[R40] 追加写日志
来源：http://wap.zdbjq.cn/Article/details/gxgmwfqeo.sHtML

echo "log" >> out.log
来源：http://read.share.zdbjq.cn/Article/details/gmkjduodj.sHtML

[R41] 丢弃输出
来源：http://baike.zdbjq.cn/Article/details/gmjgtfrgq.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/gaeovoopt.sHtML

[R42] 输入重定向
来源：http://baike.fehbvm.com/Article/details/gvmpohcfh.sHtML

wc -l < a.txt
来源：http://mobile.fehbvm.com/Article/details/ggyoebcbh.sHtML

[R43] 按名字查找文件
来源：http://mobile.hesvh.cn/Article/details/gylumtdhi.sHtML

find . -name "*.log" -type f
来源：http://read.share.zdbjq.cn/Article/details/gttvrlphh.sHtML

[R44] 按修改时间查找
来源：http://wap.zdbjq.cn/Article/details/gyhczhwym.sHtML

find . -mtime -7 -type f
来源：http://wap.fehbvm.com/Article/details/gxfhrqsqu.sHtML

[R45] 批量删除
来源：http://baike.fehbvm.com/Article/details/gmxbdzjlp.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.hesvh.cn/Article/details/gkzlaqssq.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fehbvm.com/Article/details/guqmvrqch.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.hesvh.cn/Article/details/glvkoolfr.sHtML

[R47] sed 单行替换
来源：http://www.share.hesvh.cn/Article/details/gfewijznv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.hesvh.cn/Article/details/givgadfsm.sHtML

[R48] awk 取指定列
来源：http://baike.zdbjq.cn/Article/details/gfyumebxp.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.hesvh.cn/Article/details/gjfjgeiyg.sHtML

[R49] awk 带条件
来源：http://mobile.fehbvm.com/Article/details/gaumnjwwm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.zdbjq.cn/Article/details/gcdzjuqpy.sHtML

[R50] awk 求和
来源：http://www.share.fehbvm.com/Article/details/gnqtdzczr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.hesvh.cn/Article/details/gyvfmdzij.sHtML

[R51] 排序去重取前几
来源：http://3g.zdbjq.cn/Article/details/godcvvxel.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.zdbjq.cn/Article/details/gxhmprpav.sHtML

[R52] 统计行数
来源：http://blog.zdbjq.cn/Article/details/gppnpywbj.sHtML

wc -l a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gcevesogn.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.zdbjq.cn/Article/details/goghaiujl.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.hesvh.cn/Article/details/gvsculcas.sHtML

[R54] 比较两个文件
来源：http://www.share.hesvh.cn/Article/details/gjnrxezdd.sHtML

diff a.txt b.txt
来源：http://m.share.zdbjq.cn/Article/details/gkudfesst.sHtML

[R55] 压缩与解压
来源：http://mobile.fehbvm.com/Article/details/gaiqkwqox.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.zdbjq.cn/Article/details/gffkqtxjk.sHtML

[R56] 远程拷贝
来源：http://wap.zdbjq.cn/Article/details/ggqyevyyz.sHtML

scp file user@host:/path/
来源：http://read.share.fehbvm.com/Article/details/gbbppselg.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fehbvm.com/Article/details/gcnjnejal.sHtML

ssh user@host 'uptime'
来源：http://www.share.fehbvm.com/Article/details/gmmwcoowe.sHtML

[R58] 下载文件
来源：http://blog.zdbjq.cn/Article/details/guaqajszz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.hesvh.cn/Article/details/gbfyrdkbw.sHtML

[R59] 发 POST JSON
来源：http://www.share.zdbjq.cn/Article/details/gipitxgqn.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.zdbjq.cn/Article/details/gvgmmrcvv.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/gjeqhqexi.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fehbvm.com/Article/details/gikiudpek.sHtML

[R61] 磁盘占用
来源：http://baike.zdbjq.cn/Article/details/glznhafrs.sHtML

df -h;  du -sh *
来源：http://www.share.zdbjq.cn/Article/details/gtxczytyv.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.zdbjq.cn/Article/details/ghgnkdxra.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fehbvm.com/Article/details/gomfyjjxk.sHtML

[R63] 内存与进程
来源：http://www.share.zdbjq.cn/Article/details/goilrbllk.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.hesvh.cn/Article/details/gnhxrzzrn.sHtML

[R64] 结束进程
来源：http://blog.fehbvm.com/Article/details/gwmgddprv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fehbvm.com/Article/details/gqsiyxwso.sHtML

[R65] 查看端口占用
来源：http://3g.fehbvm.com/Article/details/gzotnpzqo.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.hesvh.cn/Article/details/gfpexuaht.sHtML

[R66] 定时任务
来源：http://www.share.zdbjq.cn/Article/details/gzxfmqqob.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.hesvh.cn/Article/details/gxjzhlwhw.sHtML

[R67] 生成随机十六进制串
来源：http://baike.hesvh.cn/Article/details/giduxpcff.sHtML

openssl rand -hex 16
来源：http://www.m.share.hesvh.cn/Article/details/gdhttoyvr.sHtML

[R68] 计算文件校验值
来源：http://read.share.fehbvm.com/Article/details/gkwdviptf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.hesvh.cn/Article/details/gvsssiqup.sHtML

[R69] 生成随机密码
来源：http://m.share.zdbjq.cn/Article/details/glvdsrutv.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fehbvm.com/Article/details/gedufhoik.sHtML

[R70] 时间戳与互转
来源：http://m.share.fehbvm.com/Article/details/gapqfndrk.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fehbvm.com/Article/details/gyhstzdew.sHtML

[R71] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gqssjhbtp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.hesvh.cn/Article/details/gngdaavtk.sHtML

[R72] 等待端口就绪
来源：http://www.share.hesvh.cn/Article/details/gqchvhzpa.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/gmgsmyyzr.sHtML

[R73] 分割大日志
来源：http://www.share.fehbvm.com/Article/details/gzwmtekys.sHtML

split -l 1000 big.log part_
来源：http://www.blog.zdbjq.cn/Article/details/gnyjqdfrd.sHtML

[R74] 批量重命名
来源：http://www.m.share.hesvh.cn/Article/details/guvdiavsf.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.hesvh.cn/Article/details/gzgaqdhmq.sHtML

[R75] 导出环境变量
来源：http://baike.hesvh.cn/Article/details/gehgpfdbi.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.zdbjq.cn/Article/details/gqeicbxvr.sHtML

[R76] 使用临时文件
来源：http://3g.zdbjq.cn/Article/details/ggzwiascn.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/grsipaokp.sHtML

[R77] 读取用户输入
来源：http://blog.zdbjq.cn/Article/details/gmqqsgzxz.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fehbvm.com/Article/details/gahurdutt.sHtML

[R78] 交互式菜单
来源：http://blog.fehbvm.com/Article/details/ghaiskzka.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.zdbjq.cn/Article/details/gjtueyauu.sHtML

[R79] 解析命令行选项
来源：http://wap.fehbvm.com/Article/details/gilmhktui.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.hesvh.cn/Article/details/gbfnfkkeg.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.zdbjq.cn/Article/details/gjwionkfi.sHtML

time ./run.sh
来源：http://m.share.zdbjq.cn/Article/details/gpprufsmm.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gyggwcnba.sHtML

S. C / C++ 专题
来源：http://baike.zdbjq.cn/Article/details/gahpahsrl.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gpidcdnja.sHtML

[S01] C：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gqjfexrgc.sHtML

#include <stdio.h>
来源：http://www.share.fehbvm.com/Article/details/gscoplfac.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fehbvm.com/Article/details/gdoorklee.sHtML

[S02] C：变量与格式化输出
来源：http://blog.zdbjq.cn/Article/details/gcexhsvwd.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.zdbjq.cn/Article/details/gcqdntxvg.sHtML

[S03] C：读入整数
来源：http://www.blog.fehbvm.com/Article/details/gkmzepijy.sHtML

int x; scanf("%d", &x);
来源：http://3g.hesvh.cn/Article/details/girvitcpz.sHtML

[S04] C：字符串复制
来源：http://mobile.fehbvm.com/Article/details/gkmsymnje.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.hesvh.cn/Article/details/gqnwsbugw.sHtML

[S05] C：字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/gpzjiqsly.sHtML

strlen(s)
来源：http://read.share.hesvh.cn/Article/details/gdeeadbxk.sHtML

[S06] C：字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gaknmwjlq.sHtML

strcmp(a, b) == 0
来源：http://baike.zdbjq.cn/Article/details/gfeiyunst.sHtML

[S07] C：数组遍历求和
来源：http://baike.zdbjq.cn/Article/details/geteohusm.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.hesvh.cn/Article/details/gcnotkgyv.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.hesvh.cn/Article/details/ghqsigrbp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.zdbjq.cn/Article/details/gaymlmqko.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.zdbjq.cn/Article/details/glywyrzog.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.zdbjq.cn/Article/details/gziviwiqz.sHtML

[S10] C：指针与解引用
来源：http://read.share.fehbvm.com/Article/details/guoybaikn.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.zdbjq.cn/Article/details/gsgrogbcz.sHtML

[S11] C：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gtfxtzdwa.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fehbvm.com/Article/details/gorimxktb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.hesvh.cn/Article/details/gqyxflpzs.sHtML

fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/guqypkwmz.sHtML

[S12] C：写文件
来源：http://www.m.share.zdbjq.cn/Article/details/gkuyouvwg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gfttbyuzx.sHtML

[S13] C：宏定义
来源：http://www.blog.hesvh.cn/Article/details/gbgrecmyv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.zdbjq.cn/Article/details/grmzsltub.sHtML

[S14] C：枚举
来源：http://m.share.zdbjq.cn/Article/details/gadinqnjz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.hesvh.cn/Article/details/gdxvcmrvd.sHtML

[S15] C：类型转换
来源：http://baike.hesvh.cn/Article/details/gpudpxczf.sHtML

(double) a / b
来源：http://blog.fehbvm.com/Article/details/gzrrslywh.sHtML

[S16] C：位操作置位
来源：http://m.share.zdbjq.cn/Article/details/ghlcpfdyy.sHtML

x |= (1 << 3);
来源：http://wap.hesvh.cn/Article/details/gsuzympqk.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fehbvm.com/Article/details/grnqypzip.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.hesvh.cn/Article/details/gdufiqfas.sHtML

[S18] C：命令行参数
来源：http://read.share.zdbjq.cn/Article/details/gskcacvnh.sHtML

int main(int argc, char **argv)
来源：http://3g.fehbvm.com/Article/details/gkbdorocd.sHtML

[S19] C：快速排序
来源：http://wap.fehbvm.com/Article/details/gvjyhkyvx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gxqseasyn.sHtML

[S20] C：二分查找
来源：http://www.share.fehbvm.com/Article/details/gwjbhserm.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/gispzznfa.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.hesvh.cn/Article/details/gkclhntpt.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.zdbjq.cn/Article/details/gzwqngyvd.sHtML

[S22] C：字符串转数字
来源：http://blog.hesvh.cn/Article/details/gwwtnzobd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.hesvh.cn/Article/details/goszhtykx.sHtML

[S23] C：随机数
来源：http://www.share.zdbjq.cn/Article/details/gppjwpcfk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fehbvm.com/Article/details/gfedtlshv.sHtML

[S24] C：获取本地时间
来源：http://blog.fehbvm.com/Article/details/gfjdthcth.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.zdbjq.cn/Article/details/gpujhdixs.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fehbvm.com/Article/details/gjogncdpw.sHtML

memcpy(dst, src, n);
来源：http://3g.fehbvm.com/Article/details/gdbxwpuuk.sHtML

[S26] C：内存清零
来源：http://baike.zdbjq.cn/Article/details/gkgvqdsqr.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.zdbjq.cn/Article/details/gmtlaivfa.sHtML

[S27] C：定义常量
来源：http://www.share.zdbjq.cn/Article/details/gqtulwqfz.sHtML

const double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gvyerqdpe.sHtML

[S28] C：静态变量
来源：http://m.share.zdbjq.cn/Article/details/galliugvd.sHtML

static int counter = 0;
来源：http://3g.zdbjq.cn/Article/details/gnexglpxm.sHtML

[S29] C：变参函数
来源：http://wap.hesvh.cn/Article/details/gxjvttiwv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fehbvm.com/Article/details/gioqwhqlj.sHtML

[S30] C：头文件保护
来源：http://wap.zdbjq.cn/Article/details/grqbbbqkt.sHtML

#ifndef X_H
来源：http://www.share.hesvh.cn/Article/details/gcnahlgbq.sHtML

#define X_H
来源：http://blog.fehbvm.com/Article/details/gesmdpbhs.sHtML

#endif
来源：http://blog.fehbvm.com/Article/details/gfhwlwqua.sHtML

[S31] C++：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gpqjkgpww.sHtML

#include <iostream>
来源：http://read.share.hesvh.cn/Article/details/gcyyzjsmu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.zdbjq.cn/Article/details/gfjznxbsi.sHtML

[S32] C++：字符串
来源：http://baike.fehbvm.com/Article/details/gcvrwbbxo.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fehbvm.com/Article/details/gmrxpqzbq.sHtML


<!-- 参考信息 -->