代发 wailian999

[Q65] 回滚事务
来源：http://www.m.share.zdbjq.cn/Article/details/gtsofqxge.sHtML

ROLLBACK;
来源：http://www.m.share.fehbvm.com/Article/details/gwrfwbfbs.sHtML

[Q66] 行锁查询
来源：http://blog.fehbvm.com/Article/details/gechhiiil.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.zdbjq.cn/Article/details/gtyckhefq.sHtML

[Q67] 设置隔离级别
来源：http://3g.hesvh.cn/Article/details/gpotwrcjl.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.hesvh.cn/Article/details/gfropujix.sHtML

[Q68] 保存点
来源：http://m.share.zdbjq.cn/Article/details/gybvezoqb.sHtML

SAVEPOINT sp1;
来源：http://www.blog.hesvh.cn/Article/details/gzyzrzdhi.sHtML

ROLLBACK TO sp1;
来源：http://mobile.zdbjq.cn/Article/details/gugvqqllg.sHtML

[Q69] 查看执行计划
来源：http://3g.hesvh.cn/Article/details/ggetajijq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.hesvh.cn/Article/details/gjstsddeq.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.hesvh.cn/Article/details/giiegrmzd.sHtML

ANALYZE TABLE users;
来源：http://read.share.hesvh.cn/Article/details/guplwzoav.sHtML

[Q71] 查看建表语句
来源：http://www.share.fehbvm.com/Article/details/gtgpoyzqx.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.hesvh.cn/Article/details/gfsekkbmb.sHtML

[Q72] 查看索引
来源：http://read.share.zdbjq.cn/Article/details/gemlmpczv.sHtML

SHOW INDEX FROM users;
来源：http://wap.fehbvm.com/Article/details/gxbqbdsyd.sHtML

[Q73] 查看表状态
来源：http://baike.hesvh.cn/Article/details/gmyimxipl.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.zdbjq.cn/Article/details/gsoggnvdj.sHtML

[Q74] 强制使用索引
来源：http://baike.hesvh.cn/Article/details/gzyrljuyb.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.hesvh.cn/Article/details/gvzmbkrln.sHtML

[Q75] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gadxuzjxl.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gvxedjcki.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.zdbjq.cn/Article/details/gfeayygyv.sHtML

[Q76] 按天统计
来源：http://www.m.share.fehbvm.com/Article/details/gujgeuhzz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.zdbjq.cn/Article/details/gnavxskyy.sHtML

[Q77] 时间加减
来源：http://www.share.zdbjq.cn/Article/details/gjvqredeo.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.zdbjq.cn/Article/details/gcxytttgn.sHtML

[Q78] 当前时间
来源：http://read.share.hesvh.cn/Article/details/ghbntvnpw.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.hesvh.cn/Article/details/gfrowtwoy.sHtML

[Q79] 字符串拼接
来源：http://www.share.fehbvm.com/Article/details/gemnjalcj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.hesvh.cn/Article/details/gvxgkpscr.sHtML

[Q80] 字符串截取
来源：http://wap.fehbvm.com/Article/details/glgjhvkhh.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fehbvm.com/Article/details/glxmbpnxb.sHtML

[Q81] 字符串替换
来源：http://read.share.fehbvm.com/Article/details/gvwbnmdcu.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fehbvm.com/Article/details/gyjfhlbte.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fehbvm.com/Article/details/gfnbqwfpd.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/grqachkcr.sHtML

[Q83] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/gchqopfsn.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gmmonmerp.sHtML

[Q84] 去除首尾空格
来源：http://www.share.hesvh.cn/Article/details/gtvkubpbe.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gnpfehlxi.sHtML

[Q85] 数值取整
来源：http://mobile.fehbvm.com/Article/details/ggyuwogeh.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.hesvh.cn/Article/details/gcgtomouk.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.zdbjq.cn/Article/details/gwwdgrlzp.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.hesvh.cn/Article/details/gcjukzsjm.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.zdbjq.cn/Article/details/gulwbpayd.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.hesvh.cn/Article/details/gjlzhpbte.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.hesvh.cn/Article/details/gedvplqei.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.zdbjq.cn/Article/details/gkutabwhj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.zdbjq.cn/Article/details/gvziwpbdk.sHtML

[Q89] 判断表是否存在
来源：http://baike.fehbvm.com/Article/details/ghgzffdwj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.hesvh.cn/Article/details/ghtqviprt.sHtML

[Q90] 生成序号列
来源：http://m.share.fehbvm.com/Article/details/ghirdkatz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.zdbjq.cn/Article/details/gzkyrpyja.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gjbmwlbog.sHtML

R. Bash 专题
来源：http://www.share.zdbjq.cn/Article/details/gtwlevfxv.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gptusimal.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fehbvm.com/Article/details/gtdkoqvah.sHtML

#!/usr/bin/env bash
来源：http://mobile.zdbjq.cn/Article/details/gvslvqrhm.sHtML

set -euo pipefail
来源：http://3g.hesvh.cn/Article/details/gzaamnngn.sHtML

[R02] 变量赋值与使用
来源：http://3g.zdbjq.cn/Article/details/gxcnxluzt.sHtML

name="Tom"; echo "$name"
来源：http://www.share.zdbjq.cn/Article/details/gwsfvuzea.sHtML

[R03] 只读变量
来源：http://wap.fehbvm.com/Article/details/gxbkrkmvz.sHtML

readonly PI=3.14
来源：http://m.share.zdbjq.cn/Article/details/gzcpxqjhz.sHtML

[R04] 位置参数
来源：http://wap.zdbjq.cn/Article/details/gzrcliuxb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.hesvh.cn/Article/details/gbsiopzwv.sHtML

[R05] 参数默认值
来源：http://read.share.fehbvm.com/Article/details/gcaegvjad.sHtML

name="${1:-default}"
来源：http://m.share.fehbvm.com/Article/details/gbxqinvde.sHtML

[R06] 判断命令是否存在
来源：http://m.share.hesvh.cn/Article/details/gznvivqqc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/gynblurnw.sHtML

[R07] if 判断文件
来源：http://3g.hesvh.cn/Article/details/gbvketwyv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.zdbjq.cn/Article/details/gixwewmjp.sHtML

[R08] 数值比较
来源：http://www.blog.fehbvm.com/Article/details/gvjlvfghy.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.zdbjq.cn/Article/details/glgtlpyfl.sHtML

[R09] 字符串比较
来源：http://wap.zdbjq.cn/Article/details/gijuhuiyi.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fehbvm.com/Article/details/gurliperu.sHtML

[R10] 正则匹配
来源：http://read.share.hesvh.cn/Article/details/ghjebnhhd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.zdbjq.cn/Article/details/gmjgwcfpy.sHtML

[R11] case 多分支
来源：http://blog.zdbjq.cn/Article/details/gguyiydvy.sHtML

case "$1" in
来源：http://read.share.fehbvm.com/Article/details/ggpubmgfc.sHtML

start) echo "启动" ;;
来源：http://baike.fehbvm.com/Article/details/gotgpnsjw.sHtML

stop)  echo "停止" ;;
来源：http://www.share.hesvh.cn/Article/details/gansiahdi.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gewkdepox.sHtML

esac
来源：http://read.share.hesvh.cn/Article/details/gjcrvaqzu.sHtML

[R12] for 遍历文件
来源：http://3g.hesvh.cn/Article/details/gduucfhtt.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fehbvm.com/Article/details/gykcctozq.sHtML

[R13] for 计数循环
来源：http://www.m.share.hesvh.cn/Article/details/gqevleylx.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/gaurvwvss.sHtML

[R14] C 风格 for
来源：http://m.share.zdbjq.cn/Article/details/gxfaigjfo.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/gzgqootpz.sHtML

[R15] while 逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gpclpsoly.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.zdbjq.cn/Article/details/glmjeeezr.sHtML

[R16] until 等待条件
来源：http://wap.fehbvm.com/Article/details/gcimlydzz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/gmxbwunsa.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.zdbjq.cn/Article/details/ghfrzhubh.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.hesvh.cn/Article/details/gnzydkvcv.sHtML

[R18] 遍历数组
来源：http://m.share.hesvh.cn/Article/details/ggvoimhgo.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.zdbjq.cn/Article/details/gpvkiwoel.sHtML

[R19] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gmyghrvbs.sHtML

echo "${#arr[@]}"
来源：http://blog.hesvh.cn/Article/details/gmeqwfvwn.sHtML

[R20] 关联数组（字典）
来源：http://baike.hesvh.cn/Article/details/gxgfyjbwz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.zdbjq.cn/Article/details/gtwvpdjar.sHtML

[R21] 字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/ghinbgzsb.sHtML

echo "${#s}"
来源：http://www.blog.hesvh.cn/Article/details/gsihniykd.sHtML

[R22] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/gyttnplhz.sHtML

echo "${s:0:5}"
来源：http://read.share.fehbvm.com/Article/details/gtqtmcmse.sHtML

[R23] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gtznkmvok.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.hesvh.cn/Article/details/gljpttuaf.sHtML

[R24] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gviyhilaw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.hesvh.cn/Article/details/gzckknnby.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.hesvh.cn/Article/details/gcqbqlrmq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fehbvm.com/Article/details/gdynuwpxo.sHtML

[R26] 命令替换
来源：http://read.share.hesvh.cn/Article/details/ggccmrqif.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fehbvm.com/Article/details/gthfqjddk.sHtML

[R27] 算术展开
来源：http://baike.zdbjq.cn/Article/details/gsvriskzw.sHtML

echo $((1 + 2 * 3))
来源：http://wap.hesvh.cn/Article/details/gwhkhuxsq.sHtML

[R28] 浮点运算
来源：http://mobile.zdbjq.cn/Article/details/gfiorlobo.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.hesvh.cn/Article/details/gufzozmlv.sHtML

[R29] 定义函数
来源：http://www.m.share.hesvh.cn/Article/details/gmhomigbb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.zdbjq.cn/Article/details/gyyrwoiyt.sHtML

[R30] 函数返回状态码
来源：http://read.share.hesvh.cn/Article/details/gvmxjjmhh.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.hesvh.cn/Article/details/gftvfczrj.sHtML

[R31] 局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gorliszfo.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcommrhml.sHtML

[R32] 参数个数校验
来源：http://3g.fehbvm.com/Article/details/gjopeyztr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/gxenumrbc.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.zdbjq.cn/Article/details/gbabbxuoh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fehbvm.com/Article/details/gucickghw.sHtML

[R34] 退出时清理
来源：http://www.share.zdbjq.cn/Article/details/gezbmkatr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/gzipqoooa.sHtML

[R35] 后台执行并等待
来源：http://wap.fehbvm.com/Article/details/gerpxyvxz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fehbvm.com/Article/details/gssrjhwhl.sHtML

[R36] 并发执行多个任务
来源：http://m.share.zdbjq.cn/Article/details/gvdyrqkwa.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fehbvm.com/Article/details/gxglnjovk.sHtML

[R37] 把输出赋给变量
来源：http://baike.zdbjq.cn/Article/details/ggzomwchd.sHtML

files=$(ls -1)
来源：http://www.share.zdbjq.cn/Article/details/gkljcxurf.sHtML

[R38] 管道串联
来源：http://read.share.zdbjq.cn/Article/details/gxtjppcur.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fehbvm.com/Article/details/gsumxlbvg.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.hesvh.cn/Article/details/gtpwkznwe.sHtML

cmd > out.log 2>&1
来源：http://baike.hesvh.cn/Article/details/gupdbsiyn.sHtML

[R40] 追加写日志
来源：http://wap.zdbjq.cn/Article/details/giudpinpa.sHtML

echo "log" >> out.log
来源：http://3g.hesvh.cn/Article/details/gyorxuawz.sHtML

[R41] 丢弃输出
来源：http://www.share.hesvh.cn/Article/details/ghyhnrjbl.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fehbvm.com/Article/details/ghnzyefxn.sHtML

[R42] 输入重定向
来源：http://www.blog.zdbjq.cn/Article/details/gjilaotrc.sHtML

wc -l < a.txt
来源：http://mobile.zdbjq.cn/Article/details/gbacwdtdz.sHtML

[R43] 按名字查找文件
来源：http://mobile.hesvh.cn/Article/details/gsxkcutkw.sHtML

find . -name "*.log" -type f
来源：http://3g.fehbvm.com/Article/details/geghcohyo.sHtML

[R44] 按修改时间查找
来源：http://www.share.hesvh.cn/Article/details/gzerjdzzl.sHtML

find . -mtime -7 -type f
来源：http://baike.hesvh.cn/Article/details/ggcpawnbt.sHtML

[R45] 批量删除
来源：http://mobile.hesvh.cn/Article/details/gykajgfrs.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.hesvh.cn/Article/details/gwodjltwj.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.zdbjq.cn/Article/details/gqbrjqssa.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.hesvh.cn/Article/details/gshbrbgro.sHtML

[R47] sed 单行替换
来源：http://mobile.fehbvm.com/Article/details/ggvvdtxfv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fehbvm.com/Article/details/gonpsiobp.sHtML

[R48] awk 取指定列
来源：http://mobile.zdbjq.cn/Article/details/ggtfhuyrv.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.zdbjq.cn/Article/details/gjenbksae.sHtML

[R49] awk 带条件
来源：http://read.share.fehbvm.com/Article/details/gqbjbeizy.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fehbvm.com/Article/details/geprrfupy.sHtML

[R50] awk 求和
来源：http://baike.zdbjq.cn/Article/details/ghidcaspz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gvclyhqse.sHtML

[R51] 排序去重取前几
来源：http://wap.hesvh.cn/Article/details/gsbgsnlwo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.hesvh.cn/Article/details/gsglkywcz.sHtML

[R52] 统计行数
来源：http://mobile.fehbvm.com/Article/details/gqdneklil.sHtML

wc -l a.txt
来源：http://blog.fehbvm.com/Article/details/gsxrgcllk.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fehbvm.com/Article/details/gulkdened.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.hesvh.cn/Article/details/gbbvgxdam.sHtML

[R54] 比较两个文件
来源：http://m.share.fehbvm.com/Article/details/gicntjwsz.sHtML

diff a.txt b.txt
来源：http://read.share.zdbjq.cn/Article/details/givolhlor.sHtML

[R55] 压缩与解压
来源：http://www.blog.fehbvm.com/Article/details/gtgpbfyiz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fehbvm.com/Article/details/goemcneuu.sHtML

[R56] 远程拷贝
来源：http://www.blog.hesvh.cn/Article/details/gwgdqurlt.sHtML

scp file user@host:/path/
来源：http://m.share.hesvh.cn/Article/details/grxhiqjef.sHtML

[R57] 远程执行命令
来源：http://www.m.share.zdbjq.cn/Article/details/gmjlhaeqs.sHtML

ssh user@host 'uptime'
来源：http://read.share.zdbjq.cn/Article/details/gqwabcupn.sHtML

[R58] 下载文件
来源：http://blog.zdbjq.cn/Article/details/gmuewxaoz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fehbvm.com/Article/details/gcmhvjtbh.sHtML

[R59] 发 POST JSON
来源：http://mobile.fehbvm.com/Article/details/gcqrbervy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.hesvh.cn/Article/details/gcwqvogbj.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/gkhksbzls.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fehbvm.com/Article/details/ghspbhetm.sHtML

[R61] 磁盘占用
来源：http://wap.fehbvm.com/Article/details/gxabtmhkr.sHtML

df -h;  du -sh *
来源：http://www.blog.hesvh.cn/Article/details/gbiljwxrf.sHtML

[R62] 找最占空间的文件
来源：http://blog.fehbvm.com/Article/details/grblusugk.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fehbvm.com/Article/details/gjyrhfywl.sHtML

[R63] 内存与进程
来源：http://mobile.hesvh.cn/Article/details/grprczvrb.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.hesvh.cn/Article/details/gptclnzji.sHtML

[R64] 结束进程
来源：http://read.share.zdbjq.cn/Article/details/gfoooqoki.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.hesvh.cn/Article/details/gfabxuvwj.sHtML

[R65] 查看端口占用
来源：http://www.blog.fehbvm.com/Article/details/gylpegita.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.hesvh.cn/Article/details/gygvsvxhh.sHtML

[R66] 定时任务
来源：http://baike.hesvh.cn/Article/details/ghjnegsfj.sHtML

crontab -e;  crontab -l
来源：http://m.share.hesvh.cn/Article/details/ghxleqxks.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.hesvh.cn/Article/details/gmhtdnpnq.sHtML

openssl rand -hex 16
来源：http://3g.zdbjq.cn/Article/details/gvixwnkkk.sHtML

[R68] 计算文件校验值
来源：http://wap.zdbjq.cn/Article/details/gvytyxyhm.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.zdbjq.cn/Article/details/gczejnukb.sHtML

[R69] 生成随机密码
来源：http://baike.zdbjq.cn/Article/details/gpzepjxzi.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.hesvh.cn/Article/details/gyjommwhd.sHtML

[R70] 时间戳与互转
来源：http://blog.hesvh.cn/Article/details/gnkbdadki.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fehbvm.com/Article/details/gexfmbvth.sHtML

[R71] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/gqndokooj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fehbvm.com/Article/details/gwfbxtcyk.sHtML

[R72] 等待端口就绪
来源：http://m.share.fehbvm.com/Article/details/gwbhsflax.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/gpdcmurmy.sHtML

[R73] 分割大日志
来源：http://baike.fehbvm.com/Article/details/gxrlnkomi.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.zdbjq.cn/Article/details/gqdvxyika.sHtML

[R74] 批量重命名
来源：http://m.share.fehbvm.com/Article/details/gpinpvihs.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.hesvh.cn/Article/details/gdpgtntan.sHtML

[R75] 导出环境变量
来源：http://mobile.fehbvm.com/Article/details/gkrjgrxpb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.hesvh.cn/Article/details/gxzafqdzu.sHtML

[R76] 使用临时文件
来源：http://baike.fehbvm.com/Article/details/gkxaigjqx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.hesvh.cn/Article/details/gwcknqzee.sHtML

[R77] 读取用户输入
来源：http://mobile.zdbjq.cn/Article/details/gefqiutaw.sHtML

read -rp "请输入: " ans
来源：http://www.blog.zdbjq.cn/Article/details/guklfutfl.sHtML

[R78] 交互式菜单
来源：http://www.share.fehbvm.com/Article/details/gbzubtwdi.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.zdbjq.cn/Article/details/ghsspboak.sHtML

[R79] 解析命令行选项
来源：http://3g.zdbjq.cn/Article/details/gfdydnbzt.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fehbvm.com/Article/details/gfmivopux.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fehbvm.com/Article/details/gthaoyzyx.sHtML

time ./run.sh
来源：http://www.share.fehbvm.com/Article/details/gabsxvdfi.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/glpubjarj.sHtML

S. C / C++ 专题
来源：http://baike.hesvh.cn/Article/details/gilcjtudr.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gqlaxbjmy.sHtML

[S01] C：Hello World
来源：http://read.share.hesvh.cn/Article/details/gngvstxqg.sHtML

#include <stdio.h>
来源：http://baike.zdbjq.cn/Article/details/gvkozveyc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fehbvm.com/Article/details/gtrcfwjql.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fehbvm.com/Article/details/gneatckmj.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fehbvm.com/Article/details/grcgjaslu.sHtML

[S03] C：读入整数
来源：http://3g.fehbvm.com/Article/details/glwiyqldq.sHtML

int x; scanf("%d", &x);
来源：http://read.share.zdbjq.cn/Article/details/gxekavpps.sHtML

[S04] C：字符串复制
来源：http://baike.fehbvm.com/Article/details/gvurrhepi.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.zdbjq.cn/Article/details/gzvichnum.sHtML

[S05] C：字符串长度
来源：http://baike.fehbvm.com/Article/details/gllvsuiaf.sHtML

strlen(s)
来源：http://mobile.fehbvm.com/Article/details/gsrpcrjtz.sHtML

[S06] C：字符串比较
来源：http://read.share.hesvh.cn/Article/details/gaudwsmir.sHtML

strcmp(a, b) == 0
来源：http://mobile.hesvh.cn/Article/details/gzgxentuq.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.hesvh.cn/Article/details/gxpelvwxe.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.zdbjq.cn/Article/details/gvywufhsn.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fehbvm.com/Article/details/ghtvwwcjz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fehbvm.com/Article/details/gqvqsuzlw.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.hesvh.cn/Article/details/gbapuueut.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fehbvm.com/Article/details/gtbeavrai.sHtML

[S10] C：指针与解引用
来源：http://wap.zdbjq.cn/Article/details/gmwppkoqs.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.zdbjq.cn/Article/details/gqmfwtxop.sHtML

[S11] C：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gawhfkwau.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.zdbjq.cn/Article/details/gnpasommj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fehbvm.com/Article/details/gmedanpuk.sHtML

fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/gtzzpwktz.sHtML

[S12] C：写文件
来源：http://wap.hesvh.cn/Article/details/gvlexfqig.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gozlbptls.sHtML

[S13] C：宏定义
来源：http://www.blog.hesvh.cn/Article/details/gomlzzgqf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fehbvm.com/Article/details/gdbfdnxsr.sHtML

[S14] C：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gdzkvryng.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.hesvh.cn/Article/details/gfspkmclh.sHtML

[S15] C：类型转换
来源：http://blog.zdbjq.cn/Article/details/ggorbnytq.sHtML

(double) a / b
来源：http://mobile.zdbjq.cn/Article/details/gltxepzjp.sHtML

[S16] C：位操作置位
来源：http://m.share.zdbjq.cn/Article/details/gvlsyasqs.sHtML

x |= (1 << 3);
来源：http://read.share.fehbvm.com/Article/details/ghsktqwxs.sHtML

[S17] C：安全拼接字符串
来源：http://blog.hesvh.cn/Article/details/gbbvxtawy.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fehbvm.com/Article/details/gvozwodaw.sHtML

[S18] C：命令行参数
来源：http://3g.zdbjq.cn/Article/details/gamrbivdm.sHtML

int main(int argc, char **argv)
来源：http://mobile.fehbvm.com/Article/details/gkkkjthhc.sHtML

[S19] C：快速排序
来源：http://baike.fehbvm.com/Article/details/gtkpcyagq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/gprcgtepi.sHtML

[S20] C：二分查找
来源：http://blog.fehbvm.com/Article/details/gicdguzty.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/gbtwowazi.sHtML

[S21] C：字符类别判断
来源：http://3g.zdbjq.cn/Article/details/gndyloacr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.zdbjq.cn/Article/details/gsgqvvugm.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fehbvm.com/Article/details/grojvdkdj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.zdbjq.cn/Article/details/gzclhvspf.sHtML

[S23] C：随机数
来源：http://m.share.zdbjq.cn/Article/details/gdwlsdzrc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.zdbjq.cn/Article/details/gfmmhrraw.sHtML

[S24] C：获取本地时间
来源：http://read.share.zdbjq.cn/Article/details/gajgccdgh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fehbvm.com/Article/details/gyljwokni.sHtML

[S25] C：内存拷贝
来源：http://m.share.hesvh.cn/Article/details/gpdctyqxl.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.zdbjq.cn/Article/details/grtajsmoi.sHtML

[S26] C：内存清零
来源：http://www.m.share.hesvh.cn/Article/details/gtucqboos.sHtML

memset(a, 0, sizeof a);
来源：http://baike.zdbjq.cn/Article/details/ghobktolb.sHtML

[S27] C：定义常量
来源：http://www.share.zdbjq.cn/Article/details/gyaenknop.sHtML

const double PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gwquectya.sHtML

[S28] C：静态变量
来源：http://m.share.zdbjq.cn/Article/details/gakrvshnl.sHtML

static int counter = 0;
来源：http://www.blog.hesvh.cn/Article/details/gvkmbyrev.sHtML

[S29] C：变参函数
来源：http://read.share.fehbvm.com/Article/details/gkizzzqur.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fehbvm.com/Article/details/ghmmkdhah.sHtML

[S30] C：头文件保护
来源：http://m.share.hesvh.cn/Article/details/gozbdbmmq.sHtML

#ifndef X_H
来源：http://www.blog.zdbjq.cn/Article/details/glvodwlrg.sHtML

#define X_H
来源：http://m.share.fehbvm.com/Article/details/gvtvflipl.sHtML

#endif
来源：http://3g.hesvh.cn/Article/details/ghjfdrlib.sHtML

[S31] C++：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gpiomewml.sHtML

#include <iostream>
来源：http://www.share.zdbjq.cn/Article/details/galciigub.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.hesvh.cn/Article/details/grkqhzcaa.sHtML

[S32] C++：字符串
来源：http://wap.hesvh.cn/Article/details/geubcxguv.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fehbvm.com/Article/details/gqnkgplvj.sHtML

[S33] C++：vector 增删
来源：http://baike.hesvh.cn/Article/details/gepogzgcp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fehbvm.com/Article/details/goetistel.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.hesvh.cn/Article/details/gsfqdfiyk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.hesvh.cn/Article/details/gwoxazshf.sHtML


<!-- 参考信息 -->