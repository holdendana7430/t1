代发 wailian999

[Q63] 开启事务
来源：http://www.share.hesvh.cn/Article/details/gghtmcvrk.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.hesvh.cn/Article/details/gghsordco.sHtML

[Q64] 提交事务
来源：http://read.share.fehbvm.com/Article/details/gbigyjwfl.sHtML

COMMIT;
来源：http://mobile.hesvh.cn/Article/details/gezjcrnbn.sHtML

[Q65] 回滚事务
来源：http://wap.fehbvm.com/Article/details/gsmknbnmj.sHtML

ROLLBACK;
来源：http://www.share.fehbvm.com/Article/details/gqeckmdtc.sHtML

[Q66] 行锁查询
来源：http://wap.fehbvm.com/Article/details/gmuwjszlx.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.zdbjq.cn/Article/details/gwfczpfts.sHtML

[Q67] 设置隔离级别
来源：http://3g.hesvh.cn/Article/details/gvkmzstmn.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.hesvh.cn/Article/details/gkqxeyarq.sHtML

[Q68] 保存点
来源：http://mobile.hesvh.cn/Article/details/gpaxlmndd.sHtML

SAVEPOINT sp1;
来源：http://mobile.hesvh.cn/Article/details/gnluporsa.sHtML

ROLLBACK TO sp1;
来源：http://www.share.zdbjq.cn/Article/details/gpihuanqi.sHtML

[Q69] 查看执行计划
来源：http://3g.hesvh.cn/Article/details/gztdriuun.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fehbvm.com/Article/details/gidgjqugc.sHtML

[Q70] 更新统计信息
来源：http://mobile.hesvh.cn/Article/details/gtonhjurw.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fehbvm.com/Article/details/ghyprwqkk.sHtML

[Q71] 查看建表语句
来源：http://3g.zdbjq.cn/Article/details/guzcifjmm.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.zdbjq.cn/Article/details/glepkrbhw.sHtML

[Q72] 查看索引
来源：http://blog.fehbvm.com/Article/details/gurhxynmh.sHtML

SHOW INDEX FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gfyogwqnn.sHtML

[Q73] 查看表状态
来源：http://blog.zdbjq.cn/Article/details/ggotyijld.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fehbvm.com/Article/details/gtjexugmk.sHtML

[Q74] 强制使用索引
来源：http://wap.hesvh.cn/Article/details/grofkpogz.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.hesvh.cn/Article/details/gfivavnig.sHtML

[Q75] 日期格式化
来源：http://baike.hesvh.cn/Article/details/gdoajqerv.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.hesvh.cn/Article/details/gowylzlvj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.zdbjq.cn/Article/details/gjgryullt.sHtML

[Q76] 按天统计
来源：http://blog.zdbjq.cn/Article/details/gepslucoc.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.hesvh.cn/Article/details/gjyilptav.sHtML

[Q77] 时间加减
来源：http://blog.hesvh.cn/Article/details/gatcmyzcj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.zdbjq.cn/Article/details/gjbayecfl.sHtML

[Q78] 当前时间
来源：http://www.m.share.fehbvm.com/Article/details/guqtxyibd.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.zdbjq.cn/Article/details/ghgnzzmot.sHtML

[Q79] 字符串拼接
来源：http://3g.hesvh.cn/Article/details/gnfabmvjv.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.hesvh.cn/Article/details/gxyxwjbpd.sHtML

[Q80] 字符串截取
来源：http://3g.fehbvm.com/Article/details/gkinbfmtl.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fehbvm.com/Article/details/gzbuohaog.sHtML

[Q81] 字符串替换
来源：http://read.share.zdbjq.cn/Article/details/ghfsneoto.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.zdbjq.cn/Article/details/gtwcuzwge.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.zdbjq.cn/Article/details/ghtmxnozk.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/guvyffdsh.sHtML

[Q83] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/gpgdwrhqs.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gmnwdpswy.sHtML

[Q84] 去除首尾空格
来源：http://m.share.hesvh.cn/Article/details/gfnisachr.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gqfqzlifc.sHtML

[Q85] 数值取整
来源：http://3g.fehbvm.com/Article/details/gkotluidw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.hesvh.cn/Article/details/ggphkmepn.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.zdbjq.cn/Article/details/gamaxzyrx.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.hesvh.cn/Article/details/gxokbjthw.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fehbvm.com/Article/details/gougtretx.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.zdbjq.cn/Article/details/gcuttcvjc.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.hesvh.cn/Article/details/gdukptuzs.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fehbvm.com/Article/details/gnckepecl.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.hesvh.cn/Article/details/grjkmahth.sHtML

[Q89] 判断表是否存在
来源：http://blog.hesvh.cn/Article/details/gserekjzn.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fehbvm.com/Article/details/geijbcdgl.sHtML

[Q90] 生成序号列
来源：http://www.share.hesvh.cn/Article/details/gftyzuoko.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fehbvm.com/Article/details/gbwxuurgh.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gtaffokyn.sHtML

R. Bash 专题
来源：http://www.share.hesvh.cn/Article/details/gpkmjvcex.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gzsuemtum.sHtML

[R01] shebang 与严格模式
来源：http://mobile.zdbjq.cn/Article/details/gpkosnofl.sHtML

#!/usr/bin/env bash
来源：http://blog.fehbvm.com/Article/details/guycxnakm.sHtML

set -euo pipefail
来源：http://baike.fehbvm.com/Article/details/gmvhzmaqx.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fehbvm.com/Article/details/gyilcwqsi.sHtML

name="Tom"; echo "$name"
来源：http://blog.hesvh.cn/Article/details/gntamtgpp.sHtML

[R03] 只读变量
来源：http://mobile.zdbjq.cn/Article/details/ghzxvtbap.sHtML

readonly PI=3.14
来源：http://m.share.zdbjq.cn/Article/details/gyjwcxvnd.sHtML

[R04] 位置参数
来源：http://www.share.zdbjq.cn/Article/details/gmnxzgwjx.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fehbvm.com/Article/details/gfagzepzl.sHtML

[R05] 参数默认值
来源：http://baike.fehbvm.com/Article/details/gpdqhtlgo.sHtML

name="${1:-default}"
来源：http://www.share.zdbjq.cn/Article/details/gzngsvqqa.sHtML

[R06] 判断命令是否存在
来源：http://blog.hesvh.cn/Article/details/gdspdelpz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/gpysywabk.sHtML

[R07] if 判断文件
来源：http://wap.hesvh.cn/Article/details/gojkyzmsg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fehbvm.com/Article/details/gwaluynhj.sHtML

[R08] 数值比较
来源：http://www.m.share.hesvh.cn/Article/details/gwengbykh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fehbvm.com/Article/details/gxchazrwf.sHtML

[R09] 字符串比较
来源：http://blog.hesvh.cn/Article/details/gbfhxbrak.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.hesvh.cn/Article/details/gykzdbvjt.sHtML

[R10] 正则匹配
来源：http://baike.zdbjq.cn/Article/details/gyaofkytu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gwvwanotb.sHtML

[R11] case 多分支
来源：http://www.share.zdbjq.cn/Article/details/gvxldspnk.sHtML

case "$1" in
来源：http://blog.fehbvm.com/Article/details/gexoplpnf.sHtML

start) echo "启动" ;;
来源：http://read.share.zdbjq.cn/Article/details/gwvqkmrka.sHtML

stop)  echo "停止" ;;
来源：http://blog.hesvh.cn/Article/details/gmujmycpa.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fehbvm.com/Article/details/gadbxhsvc.sHtML

esac
来源：http://3g.fehbvm.com/Article/details/ggztrtlaf.sHtML

[R12] for 遍历文件
来源：http://baike.zdbjq.cn/Article/details/grhjooqjy.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.hesvh.cn/Article/details/gbhjkbxnu.sHtML

[R13] for 计数循环
来源：http://3g.fehbvm.com/Article/details/grrdgjfgm.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/gkdujqzxm.sHtML

[R14] C 风格 for
来源：http://www.m.share.hesvh.cn/Article/details/gjngseziq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/gmpjuamte.sHtML

[R15] while 逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gamzurvkz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.hesvh.cn/Article/details/gkuzhqfuf.sHtML

[R16] until 等待条件
来源：http://www.share.zdbjq.cn/Article/details/ghzelnaht.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/gqnmvscgt.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fehbvm.com/Article/details/gkjyydjio.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.zdbjq.cn/Article/details/gudnlfagb.sHtML

[R18] 遍历数组
来源：http://www.m.share.fehbvm.com/Article/details/gshwyajry.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fehbvm.com/Article/details/gtpcchnkl.sHtML

[R19] 数组长度
来源：http://baike.fehbvm.com/Article/details/gjjinayay.sHtML

echo "${#arr[@]}"
来源：http://m.share.zdbjq.cn/Article/details/grbbfbuho.sHtML

[R20] 关联数组（字典）
来源：http://mobile.zdbjq.cn/Article/details/gyonczrsb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.hesvh.cn/Article/details/gzinhlwid.sHtML

[R21] 字符串长度
来源：http://www.share.zdbjq.cn/Article/details/geejkqleq.sHtML

echo "${#s}"
来源：http://blog.zdbjq.cn/Article/details/giukhihqs.sHtML

[R22] 截取子串
来源：http://baike.fehbvm.com/Article/details/gsrededsz.sHtML

echo "${s:0:5}"
来源：http://www.m.share.hesvh.cn/Article/details/gjwhrhovm.sHtML

[R23] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gkpyehkfr.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.hesvh.cn/Article/details/gbakbuvus.sHtML

[R24] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/gqsvasmay.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.zdbjq.cn/Article/details/gcqccudlz.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fehbvm.com/Article/details/gtvnprkwc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.hesvh.cn/Article/details/gmldmylrz.sHtML

[R26] 命令替换
来源：http://baike.fehbvm.com/Article/details/gqakecywm.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fehbvm.com/Article/details/gtblcxgrq.sHtML

[R27] 算术展开
来源：http://www.share.fehbvm.com/Article/details/gpuryrejv.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fehbvm.com/Article/details/gfxsxcaql.sHtML

[R28] 浮点运算
来源：http://www.share.fehbvm.com/Article/details/gpjbawlqa.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.hesvh.cn/Article/details/gkysjpdir.sHtML

[R29] 定义函数
来源：http://m.share.hesvh.cn/Article/details/gxydhhcli.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.zdbjq.cn/Article/details/gcfotwnay.sHtML

[R30] 函数返回状态码
来源：http://m.share.hesvh.cn/Article/details/galiuungo.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fehbvm.com/Article/details/gpkkfdkux.sHtML

[R31] 局部变量
来源：http://www.share.zdbjq.cn/Article/details/gkbqnepxj.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.zdbjq.cn/Article/details/grrotqaro.sHtML

[R32] 参数个数校验
来源：http://www.m.share.zdbjq.cn/Article/details/gjkhwpsxy.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/gaaxwmyhw.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fehbvm.com/Article/details/gxltrecbn.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.zdbjq.cn/Article/details/geclfsjqe.sHtML

[R34] 退出时清理
来源：http://3g.zdbjq.cn/Article/details/gerevpcad.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.zdbjq.cn/Article/details/gsoejoccd.sHtML

[R35] 后台执行并等待
来源：http://m.share.hesvh.cn/Article/details/ghodshlcg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.zdbjq.cn/Article/details/grkifpqel.sHtML

[R36] 并发执行多个任务
来源：http://wap.fehbvm.com/Article/details/gkctlltng.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.hesvh.cn/Article/details/gcofoeglg.sHtML

[R37] 把输出赋给变量
来源：http://www.share.zdbjq.cn/Article/details/gygwzarft.sHtML

files=$(ls -1)
来源：http://www.share.zdbjq.cn/Article/details/geonajlen.sHtML

[R38] 管道串联
来源：http://mobile.fehbvm.com/Article/details/ghnwyaoqj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.zdbjq.cn/Article/details/gcfxkgubr.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fehbvm.com/Article/details/gdmunzzfm.sHtML

cmd > out.log 2>&1
来源：http://mobile.hesvh.cn/Article/details/gvmzfnbtp.sHtML

[R40] 追加写日志
来源：http://read.share.fehbvm.com/Article/details/ghwdewxea.sHtML

echo "log" >> out.log
来源：http://m.share.zdbjq.cn/Article/details/gkfxqdfuf.sHtML

[R41] 丢弃输出
来源：http://3g.fehbvm.com/Article/details/gzhukiabr.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.hesvh.cn/Article/details/gkahokxeo.sHtML

[R42] 输入重定向
来源：http://www.share.hesvh.cn/Article/details/gezipivbd.sHtML

wc -l < a.txt
来源：http://www.m.share.fehbvm.com/Article/details/ggeikccip.sHtML

[R43] 按名字查找文件
来源：http://3g.hesvh.cn/Article/details/ggtdospaa.sHtML

find . -name "*.log" -type f
来源：http://mobile.hesvh.cn/Article/details/gldsxjrmv.sHtML

[R44] 按修改时间查找
来源：http://blog.fehbvm.com/Article/details/gbifknxhz.sHtML

find . -mtime -7 -type f
来源：http://www.share.zdbjq.cn/Article/details/gvrisosyz.sHtML

[R45] 批量删除
来源：http://wap.hesvh.cn/Article/details/gttqbownq.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fehbvm.com/Article/details/gfvnnbrgi.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fehbvm.com/Article/details/gjejqnrhh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.zdbjq.cn/Article/details/gdvzvmkkm.sHtML

[R47] sed 单行替换
来源：http://blog.fehbvm.com/Article/details/gqephvopt.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.hesvh.cn/Article/details/ggixrjqyz.sHtML

[R48] awk 取指定列
来源：http://3g.fehbvm.com/Article/details/gdgzzqcag.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.hesvh.cn/Article/details/gnihkjqtz.sHtML

[R49] awk 带条件
来源：http://www.m.share.zdbjq.cn/Article/details/grmgjclkt.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fehbvm.com/Article/details/graaccpqk.sHtML

[R50] awk 求和
来源：http://read.share.hesvh.cn/Article/details/gjqxfuwou.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.hesvh.cn/Article/details/ghgwgackv.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.hesvh.cn/Article/details/gkveazewm.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.hesvh.cn/Article/details/gyinahyjj.sHtML

[R52] 统计行数
来源：http://wap.zdbjq.cn/Article/details/gllgadcfx.sHtML

wc -l a.txt
来源：http://3g.hesvh.cn/Article/details/gyezbybfh.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.zdbjq.cn/Article/details/guenwqujc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.hesvh.cn/Article/details/goecrdnwv.sHtML

[R54] 比较两个文件
来源：http://3g.hesvh.cn/Article/details/gpgrietej.sHtML

diff a.txt b.txt
来源：http://read.share.fehbvm.com/Article/details/ghjzwiosh.sHtML

[R55] 压缩与解压
来源：http://wap.fehbvm.com/Article/details/gjpwaxpdk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fehbvm.com/Article/details/gscrklysc.sHtML

[R56] 远程拷贝
来源：http://read.share.hesvh.cn/Article/details/glssytrst.sHtML

scp file user@host:/path/
来源：http://baike.hesvh.cn/Article/details/gyauchhjj.sHtML

[R57] 远程执行命令
来源：http://blog.zdbjq.cn/Article/details/gaqozezgo.sHtML

ssh user@host 'uptime'
来源：http://wap.fehbvm.com/Article/details/gvikhpftz.sHtML

[R58] 下载文件
来源：http://blog.zdbjq.cn/Article/details/gjuhtxvqb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.zdbjq.cn/Article/details/ghgmcogtx.sHtML

[R59] 发 POST JSON
来源：http://mobile.fehbvm.com/Article/details/gqxetbubc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.hesvh.cn/Article/details/gjdyfmcmh.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/gihjdjvst.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.zdbjq.cn/Article/details/grifjjgtd.sHtML

[R61] 磁盘占用
来源：http://www.m.share.zdbjq.cn/Article/details/gboklbzbq.sHtML

df -h;  du -sh *
来源：http://www.m.share.hesvh.cn/Article/details/gqbklniqx.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fehbvm.com/Article/details/ggmrolmdt.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.zdbjq.cn/Article/details/guvrexmuj.sHtML

[R63] 内存与进程
来源：http://blog.fehbvm.com/Article/details/gxxsquzah.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.hesvh.cn/Article/details/gsiiidlug.sHtML

[R64] 结束进程
来源：http://read.share.zdbjq.cn/Article/details/gmdvvxqds.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fehbvm.com/Article/details/gxzitnlke.sHtML

[R65] 查看端口占用
来源：http://3g.hesvh.cn/Article/details/gkrucwmwa.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.zdbjq.cn/Article/details/guetmlbge.sHtML

[R66] 定时任务
来源：http://m.share.fehbvm.com/Article/details/gogkltbta.sHtML

crontab -e;  crontab -l
来源：http://baike.zdbjq.cn/Article/details/gpoemxcya.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fehbvm.com/Article/details/gioxncqhj.sHtML

openssl rand -hex 16
来源：http://www.blog.fehbvm.com/Article/details/gyisdjomu.sHtML

[R68] 计算文件校验值
来源：http://www.blog.zdbjq.cn/Article/details/gckksbacx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.hesvh.cn/Article/details/gmagvfdzm.sHtML

[R69] 生成随机密码
来源：http://baike.hesvh.cn/Article/details/guoiyoqws.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.zdbjq.cn/Article/details/ghfimdsbi.sHtML

[R70] 时间戳与互转
来源：http://www.blog.hesvh.cn/Article/details/gdoeouowt.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.hesvh.cn/Article/details/gptdtfund.sHtML

[R71] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gihhjshja.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fehbvm.com/Article/details/gadfuknnp.sHtML

[R72] 等待端口就绪
来源：http://www.share.hesvh.cn/Article/details/gmtylrxif.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/ghxthepvd.sHtML

[R73] 分割大日志
来源：http://3g.fehbvm.com/Article/details/gwtjylkfi.sHtML

split -l 1000 big.log part_
来源：http://mobile.fehbvm.com/Article/details/ghvyfjjom.sHtML

[R74] 批量重命名
来源：http://www.m.share.fehbvm.com/Article/details/gavucbenj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fehbvm.com/Article/details/gcawxdwis.sHtML

[R75] 导出环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gtswbwqjp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.zdbjq.cn/Article/details/gcihqaqrl.sHtML

[R76] 使用临时文件
来源：http://3g.zdbjq.cn/Article/details/gkfaddhmc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.hesvh.cn/Article/details/gimqmkqbj.sHtML

[R77] 读取用户输入
来源：http://www.blog.zdbjq.cn/Article/details/gfkozsvge.sHtML

read -rp "请输入: " ans
来源：http://wap.hesvh.cn/Article/details/glkiqsrkk.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fehbvm.com/Article/details/gvfcexhhm.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.hesvh.cn/Article/details/gpneauztr.sHtML

[R79] 解析命令行选项
来源：http://m.share.hesvh.cn/Article/details/gyxejxnhl.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.zdbjq.cn/Article/details/guzgigirc.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fehbvm.com/Article/details/ggnvbuyff.sHtML

time ./run.sh
来源：http://www.blog.fehbvm.com/Article/details/gjxbnmyzb.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gzjqwwlmi.sHtML

S. C / C++ 专题
来源：http://wap.hesvh.cn/Article/details/gluquglwt.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ggebjdiiy.sHtML

[S01] C：Hello World
来源：http://www.share.fehbvm.com/Article/details/gbmmlqfnr.sHtML

#include <stdio.h>
来源：http://m.share.hesvh.cn/Article/details/grwsjwnlo.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.hesvh.cn/Article/details/gnygzmlct.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.zdbjq.cn/Article/details/gxlndnnei.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.zdbjq.cn/Article/details/glefquvrs.sHtML

[S03] C：读入整数
来源：http://wap.hesvh.cn/Article/details/gzpwinmbx.sHtML

int x; scanf("%d", &x);
来源：http://wap.fehbvm.com/Article/details/gipjfxgyd.sHtML

[S04] C：字符串复制
来源：http://blog.zdbjq.cn/Article/details/gvbprmxwu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gmdbmgzgh.sHtML

[S05] C：字符串长度
来源：http://mobile.zdbjq.cn/Article/details/gzhwjpjrs.sHtML

strlen(s)
来源：http://m.share.zdbjq.cn/Article/details/gbxbvshez.sHtML

[S06] C：字符串比较
来源：http://3g.zdbjq.cn/Article/details/gfrsxlwja.sHtML

strcmp(a, b) == 0
来源：http://m.share.fehbvm.com/Article/details/ggawsrjkw.sHtML

[S07] C：数组遍历求和
来源：http://blog.zdbjq.cn/Article/details/ggxcisafz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fehbvm.com/Article/details/goaztmlls.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fehbvm.com/Article/details/gyewxpxkw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.zdbjq.cn/Article/details/gsvgtlnku.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.hesvh.cn/Article/details/gpbkefrlp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.zdbjq.cn/Article/details/gmhnjwpru.sHtML

[S10] C：指针与解引用
来源：http://blog.fehbvm.com/Article/details/gonmomokn.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fehbvm.com/Article/details/galfryxfh.sHtML

[S11] C：逐行读文件
来源：http://3g.fehbvm.com/Article/details/ghilnmsbq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.zdbjq.cn/Article/details/gsuoptcsy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fehbvm.com/Article/details/gsymsqbto.sHtML

fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/gktcyevzn.sHtML

[S12] C：写文件
来源：http://mobile.hesvh.cn/Article/details/godgthhqo.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/gjpskdafd.sHtML

[S13] C：宏定义
来源：http://3g.hesvh.cn/Article/details/gnthopawu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.hesvh.cn/Article/details/gyvvuyysx.sHtML

[S14] C：枚举
来源：http://wap.zdbjq.cn/Article/details/gzvmuyeuy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.zdbjq.cn/Article/details/gqvdjskqo.sHtML

[S15] C：类型转换
来源：http://m.share.zdbjq.cn/Article/details/gxmkwdcrw.sHtML

(double) a / b
来源：http://read.share.fehbvm.com/Article/details/geumjznef.sHtML

[S16] C：位操作置位
来源：http://read.share.zdbjq.cn/Article/details/gicdmwzef.sHtML

x |= (1 << 3);
来源：http://read.share.fehbvm.com/Article/details/gtbxpyoyx.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fehbvm.com/Article/details/gtvoxtkqw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.zdbjq.cn/Article/details/gqwrpsfpe.sHtML

[S18] C：命令行参数
来源：http://wap.hesvh.cn/Article/details/gtvocugma.sHtML

int main(int argc, char **argv)
来源：http://wap.fehbvm.com/Article/details/gqgmykzti.sHtML

[S19] C：快速排序
来源：http://mobile.hesvh.cn/Article/details/gvnympmby.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gygjmaxye.sHtML

[S20] C：二分查找
来源：http://read.share.fehbvm.com/Article/details/gofldernq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/gdnqxgdta.sHtML

[S21] C：字符类别判断
来源：http://www.share.zdbjq.cn/Article/details/gifzrbcde.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.hesvh.cn/Article/details/ghfxtgmwk.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.zdbjq.cn/Article/details/gcaxchzrc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fehbvm.com/Article/details/gtiswksva.sHtML

[S23] C：随机数
来源：http://mobile.zdbjq.cn/Article/details/gxvpdmkhi.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fehbvm.com/Article/details/gtwpbvlkh.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fehbvm.com/Article/details/gpzjagxop.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.hesvh.cn/Article/details/gtpewvdad.sHtML

[S25] C：内存拷贝
来源：http://read.share.fehbvm.com/Article/details/gmcoktnfg.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.hesvh.cn/Article/details/gwbxjgeuy.sHtML

[S26] C：内存清零
来源：http://mobile.hesvh.cn/Article/details/gguehyvow.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.hesvh.cn/Article/details/giemefdzz.sHtML

[S27] C：定义常量
来源：http://www.m.share.fehbvm.com/Article/details/gdhanfshy.sHtML

const double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gsqilzzva.sHtML

[S28] C：静态变量
来源：http://wap.fehbvm.com/Article/details/gnbofjbjw.sHtML

static int counter = 0;
来源：http://www.m.share.hesvh.cn/Article/details/gdkkehzfd.sHtML

[S29] C：变参函数
来源：http://www.blog.hesvh.cn/Article/details/gaiadysjt.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.hesvh.cn/Article/details/gxljavpjy.sHtML

[S30] C：头文件保护
来源：http://baike.fehbvm.com/Article/details/gmnogxnig.sHtML

#ifndef X_H
来源：http://m.share.fehbvm.com/Article/details/gvkqfnsiq.sHtML

#define X_H
来源：http://read.share.hesvh.cn/Article/details/gbqpzhhgj.sHtML

#endif
来源：http://www.blog.hesvh.cn/Article/details/gtpxctcae.sHtML

[S31] C++：Hello World
来源：http://wap.fehbvm.com/Article/details/gajiafwqg.sHtML

#include <iostream>
来源：http://blog.hesvh.cn/Article/details/glfssrlbs.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fehbvm.com/Article/details/gdqpmuuuc.sHtML

[S32] C++：字符串
来源：http://3g.fehbvm.com/Article/details/glhijrakh.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.hesvh.cn/Article/details/gzygqbtwj.sHtML


<!-- 参考信息 -->