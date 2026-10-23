代发 wailian999

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3pikifetc.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3hdyhrcyl.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3jmganhrf.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3lpnufgky.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3vtevwckz.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3vbcfydeq.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3xpkxigyw.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3ehxsgkfq.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3wuuygqwo.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rbynsuco.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3qjiakxjc.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jkyfpqhp.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3jqhholnv.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fqtpjrkx.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3blwnykdq.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3awxcqciy.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3yipcctlx.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ovllrzjd.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3ccwwxujq.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3fhcsdadr.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3thzhufbd.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3dhakjegp.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3lvkrozte.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3vwlnpbne.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3aupiworz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3zkvxjiwx.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jhhghtev.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3mfpjyire.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3ugbmdsbd.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3zglpbvrx.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3rkcuyhbw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uhwtpuct.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3thtbpcul.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3trqxvnwz.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3ooayqtmo.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3auudwobm.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3nfxpnkwb.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3nichkphh.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3imxurkth.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3qxhxjvrb.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3vkoriynk.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3dnyyqrur.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3kwcjgavh.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3bjyviytk.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3ivuqmmpo.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3rxdmliyj.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3dghrxrsh.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3rjjbpycu.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3gqtrfsia.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3cihgjwoe.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3fhazgytr.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3kzesegtf.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3jzotivde.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3nprjbala.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ojmpwsil.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3ojdyygmb.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3ffujdcne.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3grjsjkmx.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3acaryqvs.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3uwsrcvqa.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3dflzovxr.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3znlxuhaz.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3ztvdysyk.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3bvzqtqzx.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3cxidxacr.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3qdedmcza.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3fyirnepo.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ebpjrusy.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vcgpwatx.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3fyiiruvd.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3frggunkg.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3qyhnqaxb.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3gqnitijg.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3qcttbvbo.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3vxklneyi.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3puyfxchb.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3uggwptvv.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3khsdtefo.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3qwgutlct.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3txlapeji.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3sburljoc.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3ivrpmmki.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3jwqeqdhb.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3gquoktjl.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3uzvkrfaz.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3dmniqkcb.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3esvjugru.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3endtbota.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3aqzeahru.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3lcrxjbij.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3jnnrswmx.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3jtukpean.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3kvrhryty.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3gsyuhfnz.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3rgymgqyv.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3hgbfclnx.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3lcrleqsm.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3oeakmoes.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3pxztrvbe.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3oaomzzgs.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3viqwaztl.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3lxmoxjnb.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3tifsyaki.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3weeottcf.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3ffscddzh.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3wwxfxdbx.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3weozwjnf.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3uwgbtlfj.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3egermcoe.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3muuiijsv.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3ekdeiwen.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3vcdortdp.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3efhtsnzo.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3dcgbhitj.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3mdyusqaj.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3yjxlqynb.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3sbrzhain.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3amaxcway.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3xneoiqgc.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3duejjcjs.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3ddqqcmsh.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3hcgtcvcw.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3siffrzhv.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3liwgmiot.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3wjkggefg.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3mwwyfsnd.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3qtxqjiij.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3bptwhbby.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3whcjodiq.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3tjcjefun.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3grsxoeny.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3jjeymyql.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kojtsnya.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3dlaocdhg.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3asnrhtll.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3tusyktsn.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3tgvirtcd.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3gbiojkfb.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3myypjaab.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3wrdwdxga.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3jmmcapwc.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3gldxyxvm.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wtgnhcrp.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3jmkdcgum.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3tqfyzxub.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3xrdcnezv.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mkcivybw.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3zsyeljds.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3qyybajox.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3cqyoluss.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3jimfoljr.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3fivgakej.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3pkghvntv.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3yzhmjtpx.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3zczphakh.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3htbiabzf.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3acfvpklo.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3qvewbymz.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3kqstclks.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3uvejdzsn.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3uzyfxxfu.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3jtgtzbgq.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3inimlizb.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3jordckik.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3sapivmbx.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3qebmaojg.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3arqjdpup.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3ibdpgahz.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3mqngiohq.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3esgyyibp.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3hoywxexk.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3lhqzrgoz.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3jsphqlyt.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3dfkpmfal.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3jyqbhcxo.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3lgrycrov.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3hzocryve.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3zlfhhmaw.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3gutknqtt.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3bjyqvbmd.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3wilrkxif.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3ehvzlfel.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3dqwerpxk.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3lqteidqr.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3sjylermx.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3xzlxuzvw.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3eqclozrd.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3juylyuft.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3csiqsjfh.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3gxtxtsyx.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3viybmguf.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3osvtbygn.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3hshjbkds.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3oifkuvhu.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3agknxoel.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3cjfflhfa.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3dbhebyoh.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3cuvrnlvz.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3mskcavdx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cudrrtlh.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3iqcolwcd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jdocynpk.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vdohnlaj.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3dhjttdpq.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3aoheqgge.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3odoagfli.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3kuidnlcw.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3wythjvcv.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3bmbuvlhg.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3ewwfneeb.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3iukfgoji.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ulnycuwk.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uljmdecr.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3byhapmzq.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3zfufxhet.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3rocqihpr.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3ezjgfftc.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3fsfohdhv.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3eceqevhn.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3hqwrkler.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3xqqkdmrx.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3ksohmfuo.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3cabvevvt.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3wpkgtbnu.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3jydzlqmv.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3dvannpmy.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3xmlfydgm.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3hacnrsju.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3uxfzmhyw.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3exsyldjv.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3fwcyeoyf.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3dtvwgtmp.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3uzgquyjv.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3eyjeuezf.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3oqfthepc.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3tzsprodx.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3gajipfsi.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3urpqoxxc.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3nlvxzufs.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3xbkmwxux.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3hmhzbhwy.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3pbvvoigo.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3nrgcgoow.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3yycjrglf.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3losmnfqw.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3ngmtsbuq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3pmdsltio.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3wolewfze.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3doytubkh.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3luqjdpem.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3rlgakxcb.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3zticzahl.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3dxtrwinf.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3yijqdgse.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3bgrklwlz.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3ehwqaied.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3tlpuiohx.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3ihxsoqxo.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3xamemdms.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3tiqorihs.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3soofszpi.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3gcdonoof.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3mmcqnaie.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3yvafekbd.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3lkisnyrj.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3qegrjgkg.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3kxxqshkd.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3snhxnejf.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3gacpevvl.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3ecgnlqwu.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3fsjnpqlj.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3jjbcwngq.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3wmhoudbq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3slpyaais.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3myjwbqhz.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3vtvingyg.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3caaudnoz.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zjwvyioz.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3gxdtgkmo.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3iezvkdkv.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3zikpuirf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3gtcxtbaz.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3xgnxlbme.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3prjgwfgl.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3oxvuhqpq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3htcpoglm.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3cpzgwmwf.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vcyhawce.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3nqjxwdqh.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3ponhuxup.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3dxcidilk.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3tzrcetlh.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3kcvfpift.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3crtnwifv.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3sknhchnx.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3arktxdxn.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3ktsczjkf.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3qroscndf.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3iwumskcs.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3tbggzhhp.html


<!-- 参考信息 -->