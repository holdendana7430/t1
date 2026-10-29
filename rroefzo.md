代发 wailian999

[Q63] 开启事务
来源：http://m.share.hesvh.cn/Article/details/gcbgzfcqk.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.zdbjq.cn/Article/details/gujyrgdtw.sHtML

[Q64] 提交事务
来源：http://m.share.zdbjq.cn/Article/details/glypavdhk.sHtML

COMMIT;
来源：http://www.blog.fehbvm.com/Article/details/grqxeqhbu.sHtML

[Q65] 回滚事务
来源：http://blog.fehbvm.com/Article/details/gkgihgwjz.sHtML

ROLLBACK;
来源：http://baike.fehbvm.com/Article/details/gekjhzyes.sHtML

[Q66] 行锁查询
来源：http://baike.zdbjq.cn/Article/details/gemlgwmib.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fehbvm.com/Article/details/glipndgqh.sHtML

[Q67] 设置隔离级别
来源：http://www.share.zdbjq.cn/Article/details/gtprdwbee.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.hesvh.cn/Article/details/gtnmrmasq.sHtML

[Q68] 保存点
来源：http://blog.zdbjq.cn/Article/details/gusqioyld.sHtML

SAVEPOINT sp1;
来源：http://www.blog.zdbjq.cn/Article/details/ghcljzhaj.sHtML

ROLLBACK TO sp1;
来源：http://baike.hesvh.cn/Article/details/gnxfmbyaf.sHtML

[Q69] 查看执行计划
来源：http://www.blog.fehbvm.com/Article/details/grzuihvvg.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.zdbjq.cn/Article/details/gcucwzfbu.sHtML

[Q70] 更新统计信息
来源：http://m.share.fehbvm.com/Article/details/gkmdlvnmc.sHtML

ANALYZE TABLE users;
来源：http://baike.hesvh.cn/Article/details/gczpcdaxr.sHtML

[Q71] 查看建表语句
来源：http://wap.hesvh.cn/Article/details/ghfziiyfb.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.hesvh.cn/Article/details/gvfqgelhn.sHtML

[Q72] 查看索引
来源：http://mobile.hesvh.cn/Article/details/guxqykcfb.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fehbvm.com/Article/details/gaynhfmby.sHtML

[Q73] 查看表状态
来源：http://www.blog.hesvh.cn/Article/details/gbyatlker.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.zdbjq.cn/Article/details/gpaigjctl.sHtML

[Q74] 强制使用索引
来源：http://baike.fehbvm.com/Article/details/ggubirplm.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.zdbjq.cn/Article/details/gtqrowldy.sHtML

[Q75] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/gkvhgsdwb.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.hesvh.cn/Article/details/gudzltayq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.zdbjq.cn/Article/details/gukmfeyoq.sHtML

[Q76] 按天统计
来源：http://www.blog.fehbvm.com/Article/details/gmqamwypy.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.zdbjq.cn/Article/details/gsywjahzm.sHtML

[Q77] 时间加减
来源：http://mobile.fehbvm.com/Article/details/gzazqsbvk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.zdbjq.cn/Article/details/gfdoznpsp.sHtML

[Q78] 当前时间
来源：http://baike.zdbjq.cn/Article/details/gatrqqkkf.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.zdbjq.cn/Article/details/gbuevtfqc.sHtML

[Q79] 字符串拼接
来源：http://3g.hesvh.cn/Article/details/gcaldxraz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.hesvh.cn/Article/details/gkdvwvlxg.sHtML

[Q80] 字符串截取
来源：http://read.share.hesvh.cn/Article/details/gkrrvmdzo.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gjfhiqrex.sHtML

[Q81] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/gxtkliinq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gmnrdvtkq.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.hesvh.cn/Article/details/gfxbkkbmc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gmdlhwmap.sHtML

[Q83] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/ghuwygetb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/glfraitmt.sHtML

[Q84] 去除首尾空格
来源：http://3g.hesvh.cn/Article/details/gxugsdafn.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gswrhcctx.sHtML

[Q85] 数值取整
来源：http://wap.zdbjq.cn/Article/details/gvxkophpc.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.hesvh.cn/Article/details/gqirqqmbe.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fehbvm.com/Article/details/gqbwkthyf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fehbvm.com/Article/details/gqjmarupf.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fehbvm.com/Article/details/gtvmabsib.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fehbvm.com/Article/details/gayyhmuiz.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.hesvh.cn/Article/details/govfkweuh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fehbvm.com/Article/details/gbyddpdqz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gaajvkdyv.sHtML

[Q89] 判断表是否存在
来源：http://wap.fehbvm.com/Article/details/ggzlycxjl.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fehbvm.com/Article/details/gnpzjpbbg.sHtML

[Q90] 生成序号列
来源：http://www.blog.zdbjq.cn/Article/details/ggcgvalht.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.zdbjq.cn/Article/details/gpllyfqhr.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gpwfvxowq.sHtML

R. Bash 专题
来源：http://3g.zdbjq.cn/Article/details/gtaomybam.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gkgkaxlpy.sHtML

[R01] shebang 与严格模式
来源：http://www.share.zdbjq.cn/Article/details/gdfzbttrg.sHtML

#!/usr/bin/env bash
来源：http://mobile.hesvh.cn/Article/details/gtykuaany.sHtML

set -euo pipefail
来源：http://blog.fehbvm.com/Article/details/gwlyvrvdr.sHtML

[R02] 变量赋值与使用
来源：http://mobile.hesvh.cn/Article/details/gyyfdumbg.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fehbvm.com/Article/details/gaiodobud.sHtML

[R03] 只读变量
来源：http://3g.fehbvm.com/Article/details/geshtkrsk.sHtML

readonly PI=3.14
来源：http://read.share.fehbvm.com/Article/details/gsylmiucz.sHtML

[R04] 位置参数
来源：http://m.share.hesvh.cn/Article/details/ggboquwdy.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fehbvm.com/Article/details/ggmbcwrbs.sHtML

[R05] 参数默认值
来源：http://m.share.zdbjq.cn/Article/details/gcatiqowj.sHtML

name="${1:-default}"
来源：http://blog.hesvh.cn/Article/details/gyseujvgc.sHtML

[R06] 判断命令是否存在
来源：http://wap.hesvh.cn/Article/details/gjkutbluj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/gipcufaac.sHtML

[R07] if 判断文件
来源：http://3g.fehbvm.com/Article/details/gfhspfhnq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.zdbjq.cn/Article/details/gfutthyjv.sHtML

[R08] 数值比较
来源：http://baike.fehbvm.com/Article/details/gyanljgog.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fehbvm.com/Article/details/goajsyghv.sHtML

[R09] 字符串比较
来源：http://read.share.fehbvm.com/Article/details/gurddpvxr.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.hesvh.cn/Article/details/goswoglpm.sHtML

[R10] 正则匹配
来源：http://www.m.share.zdbjq.cn/Article/details/glieazfro.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fehbvm.com/Article/details/gqjixkfuf.sHtML

[R11] case 多分支
来源：http://m.share.hesvh.cn/Article/details/gkyaffedz.sHtML

case "$1" in
来源：http://www.m.share.hesvh.cn/Article/details/gbqytgeow.sHtML

start) echo "启动" ;;
来源：http://3g.hesvh.cn/Article/details/gcbdbphna.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fehbvm.com/Article/details/gaxpwktdl.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gjvatdjpa.sHtML

esac
来源：http://blog.fehbvm.com/Article/details/gjruquzss.sHtML

[R12] for 遍历文件
来源：http://baike.fehbvm.com/Article/details/gpvbiyywd.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.hesvh.cn/Article/details/guclclzuk.sHtML

[R13] for 计数循环
来源：http://m.share.hesvh.cn/Article/details/gfcsuspgg.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/gkmparcgi.sHtML

[R14] C 风格 for
来源：http://www.share.fehbvm.com/Article/details/gqcbvfkpk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/gahaabxws.sHtML

[R15] while 逐行读文件
来源：http://3g.hesvh.cn/Article/details/gguxpbrpk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.zdbjq.cn/Article/details/gfevekrsx.sHtML

[R16] until 等待条件
来源：http://mobile.fehbvm.com/Article/details/gdnwbrkip.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gaetyikas.sHtML

[R17] 数组定义与取值
来源：http://read.share.hesvh.cn/Article/details/gqudkvdyl.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.hesvh.cn/Article/details/geiznzely.sHtML

[R18] 遍历数组
来源：http://blog.zdbjq.cn/Article/details/glnicqxga.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fehbvm.com/Article/details/geswjnjpo.sHtML

[R19] 数组长度
来源：http://3g.hesvh.cn/Article/details/gaylrpemr.sHtML

echo "${#arr[@]}"
来源：http://3g.fehbvm.com/Article/details/gjhyrrkbf.sHtML

[R20] 关联数组（字典）
来源：http://m.share.hesvh.cn/Article/details/gupmgtifu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fehbvm.com/Article/details/glugfgrde.sHtML

[R21] 字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gpzfwidxf.sHtML

echo "${#s}"
来源：http://3g.fehbvm.com/Article/details/goeobmtig.sHtML

[R22] 截取子串
来源：http://baike.zdbjq.cn/Article/details/ggdjymmye.sHtML

echo "${s:0:5}"
来源：http://m.share.fehbvm.com/Article/details/gbrtqtxvp.sHtML

[R23] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/glgtjfwex.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fehbvm.com/Article/details/gpknuaqsz.sHtML

[R24] 大小写转换
来源：http://3g.hesvh.cn/Article/details/gmwfarbra.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.zdbjq.cn/Article/details/gllshyhdh.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.zdbjq.cn/Article/details/gzuwboxmx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.zdbjq.cn/Article/details/gzuizczep.sHtML

[R26] 命令替换
来源：http://3g.zdbjq.cn/Article/details/gemmsdnut.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.zdbjq.cn/Article/details/gskwfyzri.sHtML

[R27] 算术展开
来源：http://3g.zdbjq.cn/Article/details/gqzeqdqaq.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fehbvm.com/Article/details/guthkyydh.sHtML

[R28] 浮点运算
来源：http://www.share.zdbjq.cn/Article/details/gnhtuyiuv.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fehbvm.com/Article/details/ggfiasrxc.sHtML

[R29] 定义函数
来源：http://read.share.zdbjq.cn/Article/details/ggosobhix.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.zdbjq.cn/Article/details/gkfpxsucq.sHtML

[R30] 函数返回状态码
来源：http://read.share.zdbjq.cn/Article/details/goxdblqku.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.zdbjq.cn/Article/details/gzcfelisy.sHtML

[R31] 局部变量
来源：http://www.m.share.fehbvm.com/Article/details/ghucurqmp.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.hesvh.cn/Article/details/ggdcwvaug.sHtML

[R32] 参数个数校验
来源：http://www.m.share.zdbjq.cn/Article/details/gszfelabd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fehbvm.com/Article/details/ggalvqtyg.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fehbvm.com/Article/details/gizwnkwfd.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.zdbjq.cn/Article/details/gcrugpdch.sHtML

[R34] 退出时清理
来源：http://3g.hesvh.cn/Article/details/gbtpfolie.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/gbneqihjw.sHtML

[R35] 后台执行并等待
来源：http://blog.zdbjq.cn/Article/details/gtbdlijef.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.zdbjq.cn/Article/details/gimgdtzws.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.hesvh.cn/Article/details/gfbscrztr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.hesvh.cn/Article/details/gtuihtisq.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.zdbjq.cn/Article/details/gaugbeqcs.sHtML

files=$(ls -1)
来源：http://blog.zdbjq.cn/Article/details/gcjjkykzk.sHtML

[R38] 管道串联
来源：http://blog.hesvh.cn/Article/details/gowfdvafm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.hesvh.cn/Article/details/gubjfcdtn.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.hesvh.cn/Article/details/gfeggelgg.sHtML

cmd > out.log 2>&1
来源：http://3g.fehbvm.com/Article/details/gkydhvdil.sHtML

[R40] 追加写日志
来源：http://m.share.hesvh.cn/Article/details/gsgixbhfc.sHtML

echo "log" >> out.log
来源：http://read.share.fehbvm.com/Article/details/gjmwawfkb.sHtML

[R41] 丢弃输出
来源：http://www.blog.zdbjq.cn/Article/details/genzgwgoo.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.hesvh.cn/Article/details/gcznpvbra.sHtML

[R42] 输入重定向
来源：http://www.blog.zdbjq.cn/Article/details/gxkpewmho.sHtML

wc -l < a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gksfxzgyj.sHtML

[R43] 按名字查找文件
来源：http://blog.fehbvm.com/Article/details/gtfeyebtg.sHtML

find . -name "*.log" -type f
来源：http://read.share.hesvh.cn/Article/details/gxasixlmb.sHtML

[R44] 按修改时间查找
来源：http://wap.hesvh.cn/Article/details/gbipepbmt.sHtML

find . -mtime -7 -type f
来源：http://www.share.zdbjq.cn/Article/details/gqaendswb.sHtML

[R45] 批量删除
来源：http://m.share.hesvh.cn/Article/details/gjqbuygnq.sHtML

find . -name "*.tmp" -delete
来源：http://blog.hesvh.cn/Article/details/gaaesbbkg.sHtML

[R46] 递归替换文件内容
来源：http://read.share.hesvh.cn/Article/details/gwixdmdiv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fehbvm.com/Article/details/glwgscrvb.sHtML

[R47] sed 单行替换
来源：http://read.share.fehbvm.com/Article/details/gyymxrvrw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.hesvh.cn/Article/details/gdepaiscy.sHtML

[R48] awk 取指定列
来源：http://www.m.share.hesvh.cn/Article/details/goxuvtjfn.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.hesvh.cn/Article/details/grceedhzk.sHtML

[R49] awk 带条件
来源：http://m.share.fehbvm.com/Article/details/gwokrekcf.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.hesvh.cn/Article/details/gowxbfnel.sHtML

[R50] awk 求和
来源：http://blog.hesvh.cn/Article/details/glrpsyjwc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gldcpnffg.sHtML

[R51] 排序去重取前几
来源：http://wap.zdbjq.cn/Article/details/gsvbhjsgb.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.zdbjq.cn/Article/details/gttxlmrzg.sHtML

[R52] 统计行数
来源：http://3g.zdbjq.cn/Article/details/gtzxjymed.sHtML

wc -l a.txt
来源：http://m.share.zdbjq.cn/Article/details/gjclwwgae.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fehbvm.com/Article/details/gnghjtgmi.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fehbvm.com/Article/details/gydvsjwbq.sHtML

[R54] 比较两个文件
来源：http://www.blog.zdbjq.cn/Article/details/gakyzvfzl.sHtML

diff a.txt b.txt
来源：http://blog.fehbvm.com/Article/details/gexlvpfnz.sHtML

[R55] 压缩与解压
来源：http://www.m.share.zdbjq.cn/Article/details/ghbfbdzrh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.zdbjq.cn/Article/details/gjpklrhyf.sHtML

[R56] 远程拷贝
来源：http://mobile.zdbjq.cn/Article/details/gmzdtmcsw.sHtML

scp file user@host:/path/
来源：http://blog.fehbvm.com/Article/details/ggbelnokn.sHtML

[R57] 远程执行命令
来源：http://3g.zdbjq.cn/Article/details/gwkaaevwj.sHtML

ssh user@host 'uptime'
来源：http://m.share.hesvh.cn/Article/details/gahzsovwv.sHtML

[R58] 下载文件
来源：http://mobile.zdbjq.cn/Article/details/gmoxsrrob.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.zdbjq.cn/Article/details/gqwudyjax.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/goyzzulgt.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.hesvh.cn/Article/details/gvzuemedy.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/garoaqxee.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.hesvh.cn/Article/details/gniaywdjm.sHtML

[R61] 磁盘占用
来源：http://m.share.fehbvm.com/Article/details/gadzstcbw.sHtML

df -h;  du -sh *
来源：http://mobile.zdbjq.cn/Article/details/glbedffmq.sHtML

[R62] 找最占空间的文件
来源：http://wap.fehbvm.com/Article/details/gpqjnceln.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.hesvh.cn/Article/details/gbzmpufil.sHtML

[R63] 内存与进程
来源：http://3g.hesvh.cn/Article/details/gjontddbu.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.hesvh.cn/Article/details/gbnjzokhk.sHtML

[R64] 结束进程
来源：http://read.share.zdbjq.cn/Article/details/gpyyytamz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fehbvm.com/Article/details/gprfwqvwd.sHtML

[R65] 查看端口占用
来源：http://www.blog.hesvh.cn/Article/details/gclwkagtu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.zdbjq.cn/Article/details/gdscdahdv.sHtML

[R66] 定时任务
来源：http://3g.zdbjq.cn/Article/details/gdmkhsxxz.sHtML

crontab -e;  crontab -l
来源：http://read.share.zdbjq.cn/Article/details/gdywuacow.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.hesvh.cn/Article/details/gcaxaxxwg.sHtML

openssl rand -hex 16
来源：http://www.m.share.zdbjq.cn/Article/details/glyikzous.sHtML

[R68] 计算文件校验值
来源：http://mobile.zdbjq.cn/Article/details/goghwtrlm.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.zdbjq.cn/Article/details/gwnemiqbw.sHtML

[R69] 生成随机密码
来源：http://mobile.zdbjq.cn/Article/details/gppziyrfr.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fehbvm.com/Article/details/grwfwddyb.sHtML

[R70] 时间戳与互转
来源：http://www.blog.zdbjq.cn/Article/details/ghsxrsrok.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fehbvm.com/Article/details/gnhspiyan.sHtML

[R71] 日期格式化
来源：http://3g.fehbvm.com/Article/details/gcictihto.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.zdbjq.cn/Article/details/ggnxnuykg.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.hesvh.cn/Article/details/gexwwhcij.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/guweserdc.sHtML

[R73] 分割大日志
来源：http://read.share.zdbjq.cn/Article/details/godsmumbf.sHtML

split -l 1000 big.log part_
来源：http://mobile.zdbjq.cn/Article/details/ggnkbvpwk.sHtML

[R74] 批量重命名
来源：http://wap.fehbvm.com/Article/details/gkxyqjdto.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.zdbjq.cn/Article/details/guvnlduth.sHtML

[R75] 导出环境变量
来源：http://3g.zdbjq.cn/Article/details/gkbmkobjm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.zdbjq.cn/Article/details/gdpuvpmgu.sHtML

[R76] 使用临时文件
来源：http://blog.zdbjq.cn/Article/details/gfixaqwtm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/grdglzood.sHtML

[R77] 读取用户输入
来源：http://mobile.zdbjq.cn/Article/details/gultvwycx.sHtML

read -rp "请输入: " ans
来源：http://www.share.zdbjq.cn/Article/details/gqmxzjzhf.sHtML

[R78] 交互式菜单
来源：http://wap.fehbvm.com/Article/details/gftapxzaf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.zdbjq.cn/Article/details/gepalkmos.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.hesvh.cn/Article/details/gniqgiuvz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.zdbjq.cn/Article/details/gdopkcbco.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fehbvm.com/Article/details/gpuamvbos.sHtML

time ./run.sh
来源：http://wap.hesvh.cn/Article/details/getjzwibe.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gzydmryvy.sHtML

S. C / C++ 专题
来源：http://www.blog.zdbjq.cn/Article/details/gdzeijbjq.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gmbcdlnaz.sHtML

[S01] C：Hello World
来源：http://www.blog.fehbvm.com/Article/details/guxxuwnqj.sHtML

#include <stdio.h>
来源：http://read.share.hesvh.cn/Article/details/ggvbtnvoj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.hesvh.cn/Article/details/gklvafkyo.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fehbvm.com/Article/details/gaqbhckja.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fehbvm.com/Article/details/glbhcujzl.sHtML

[S03] C：读入整数
来源：http://mobile.hesvh.cn/Article/details/goekvyipj.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.hesvh.cn/Article/details/gnxroxrri.sHtML

[S04] C：字符串复制
来源：http://3g.zdbjq.cn/Article/details/gelsvmkro.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.zdbjq.cn/Article/details/gyskvsheu.sHtML

[S05] C：字符串长度
来源：http://mobile.fehbvm.com/Article/details/gxjoidehm.sHtML

strlen(s)
来源：http://blog.hesvh.cn/Article/details/geprywacb.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gvrylxpqa.sHtML

strcmp(a, b) == 0
来源：http://wap.zdbjq.cn/Article/details/gqcltwfzy.sHtML

[S07] C：数组遍历求和
来源：http://wap.zdbjq.cn/Article/details/gppdjvuaa.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.zdbjq.cn/Article/details/gbkznddda.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.zdbjq.cn/Article/details/gojmfmmam.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fehbvm.com/Article/details/gaurcvncv.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.zdbjq.cn/Article/details/gbkirdcny.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.hesvh.cn/Article/details/gfnkhvwsn.sHtML

[S10] C：指针与解引用
来源：http://m.share.zdbjq.cn/Article/details/ggfylcupl.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fehbvm.com/Article/details/gqcdugpuz.sHtML

[S11] C：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gqnkvwede.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.zdbjq.cn/Article/details/gyjpwzwwg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.hesvh.cn/Article/details/guoszqknx.sHtML

fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/grjfandpe.sHtML

[S12] C：写文件
来源：http://m.share.fehbvm.com/Article/details/gupbegfdx.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.zdbjq.cn/Article/details/gilbcbtbs.sHtML

[S13] C：宏定义
来源：http://baike.hesvh.cn/Article/details/gyjnrvjsm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.hesvh.cn/Article/details/gcfxppeiw.sHtML

[S14] C：枚举
来源：http://www.m.share.hesvh.cn/Article/details/gaildchwi.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.zdbjq.cn/Article/details/gzjrlimke.sHtML

[S15] C：类型转换
来源：http://www.m.share.fehbvm.com/Article/details/gpkualylh.sHtML

(double) a / b
来源：http://www.blog.hesvh.cn/Article/details/ggcvnprsl.sHtML

[S16] C：位操作置位
来源：http://3g.zdbjq.cn/Article/details/gsrhznitr.sHtML

x |= (1 << 3);
来源：http://read.share.fehbvm.com/Article/details/gqyjintag.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gwlvuulsu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.zdbjq.cn/Article/details/gaepwnxwx.sHtML

[S18] C：命令行参数
来源：http://baike.zdbjq.cn/Article/details/gayzlqugc.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fehbvm.com/Article/details/gszrcipya.sHtML

[S19] C：快速排序
来源：http://www.share.zdbjq.cn/Article/details/ghdgmixzm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/gxdspzsee.sHtML

[S20] C：二分查找
来源：http://wap.fehbvm.com/Article/details/gnpzvlwya.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gisiszays.sHtML

[S21] C：字符类别判断
来源：http://www.blog.zdbjq.cn/Article/details/gypefgjdp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.hesvh.cn/Article/details/gvmndkkql.sHtML

[S22] C：字符串转数字
来源：http://read.share.zdbjq.cn/Article/details/glasoroha.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.zdbjq.cn/Article/details/giwphnici.sHtML

[S23] C：随机数
来源：http://wap.hesvh.cn/Article/details/guyhbtigg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.zdbjq.cn/Article/details/gvmojflfh.sHtML

[S24] C：获取本地时间
来源：http://3g.zdbjq.cn/Article/details/gahfsguvn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fehbvm.com/Article/details/grfvybqwe.sHtML

[S25] C：内存拷贝
来源：http://mobile.hesvh.cn/Article/details/geynnxmqg.sHtML

memcpy(dst, src, n);
来源：http://m.share.fehbvm.com/Article/details/gtdysfzmg.sHtML

[S26] C：内存清零
来源：http://mobile.hesvh.cn/Article/details/gzuswzatw.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fehbvm.com/Article/details/gqkpwrzfy.sHtML

[S27] C：定义常量
来源：http://www.blog.fehbvm.com/Article/details/ghufqkcgf.sHtML

const double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gdkanswbd.sHtML

[S28] C：静态变量
来源：http://wap.hesvh.cn/Article/details/gtwjsckwc.sHtML

static int counter = 0;
来源：http://www.blog.fehbvm.com/Article/details/gpabktlhm.sHtML

[S29] C：变参函数
来源：http://www.m.share.fehbvm.com/Article/details/gkqpgpoql.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fehbvm.com/Article/details/gzavsjizt.sHtML

[S30] C：头文件保护
来源：http://mobile.zdbjq.cn/Article/details/ggtdektvt.sHtML

#ifndef X_H
来源：http://www.share.zdbjq.cn/Article/details/gzsjpgxmy.sHtML

#define X_H
来源：http://blog.fehbvm.com/Article/details/gzitnhscz.sHtML

#endif
来源：http://blog.hesvh.cn/Article/details/gtdvgcxif.sHtML

[S31] C++：Hello World
来源：http://www.share.hesvh.cn/Article/details/gkehtvafx.sHtML

#include <iostream>
来源：http://read.share.zdbjq.cn/Article/details/gpmukepza.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.hesvh.cn/Article/details/gkxrhpwsr.sHtML

[S32] C++：字符串
来源：http://blog.zdbjq.cn/Article/details/gqhwdeknl.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.hesvh.cn/Article/details/gmbgepsjm.sHtML


<!-- 参考信息 -->